SpringScan REST API's
=====================


Login
-----

Aim is to generate a JWT token , which will be used for all further API calls. 

Client needs to send JWT token in the header, along with client Token to successfully OCR and verify the docs.

**Path** : /auth/login

**Method** : POST

**Body** : { email, password }

**Example Request**
 	.. code::
		
		curl -X POST \
		  https://api-dev.springscan.springverify.com/auth/login \
		  -H 'Content-Type: application/x-www-form-urlencoded' \
		  -H 'Postman-Token: 3027720f-71ef-4877-b851-8745e650b4c5' \
		  -H 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		  -H 'cache-control: no-cache' \
		  -d 'email=test%40springscan.com&password=springscan'

**Example Response**
	.. code::

		{
	    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3RAc3ByaW5nc2Nhbi5jb20iLCJ1c2VySWQiOiI1ZTMwN2IwNGNkNWQ5YTAzMTgwYzMwYWMiLCJpYXQiOjE1ODM0MDQzMzMsImV4cCI6MTU5MjA0NDMzM30.V_yzdNB4w5H7FAW1oc_M7iy-_-RJXOTbD8RG4erdINU",
	    "userId": "5e307b04cd5d9a03180c30ac",
	    "user_name": "klsjdskl",
	    "company_name": ""
		}

**Query Parameters**
	
	* email (string): Email registered in springscan. 
	* password (string): Password registered in springscan.


Upload Documents
----------------

This API is to be used if your platform does not have the document (JPG, JPEG, PNG etc) on a hosted URLs. 
 
We aim to provide clients with option to host their documents with us. The mentioned documents will be hosted **securely** with us.


**Path** : /user/person/upload/

**Method** : POST
		
**Example Request**
 	.. code::
		
		curl -X POST \
		  https://api-dev.springscan.springverify.com/user/person/upload/ \
		  -H 'Content-Type: image/*' \
		  -H 'Postman-Token: 0ab04006-a0b8-408e-ab8c-74fb5cb13951' \
		  -H 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		  -H 'cache-control: no-cache' \
		  -H 'content-type: multipart/form-data; boundary=----WebKitFormBoundary7MA4YWxkTrZu0gW' \
		  -F person_id=5df35fa819bd2a8d8663371c \
		  -F 'ind_aadhaar=@/Users/karanahuja/Documents/My IDs/aadhaar.png'


**Query Parameters**

 	* Header: Client Token and Auth Token
 	* face_image (optional): Selfie file
 	* ind_aadhaar (Optional): Aadhaar file
 	* personId (Optional): person id
 	* ind_pan (Optional): Pan url
 	* ind_voter_id (Optional): Voter ID file
 	* ind_driving_license (Optional): DL file
 	* ind_passport (Optional): Passport file

Initialize API
--------------

This API is used to initialize a **Person** with us. The person is initialized with or without a selfie and **any one** document. You can update or add different document later for the same person.

.. note:: 
	**Call Once**:
	Call Initialize only once in Person's lifecycle. Any subsequent calls for same person will be rejected.


.. note:: 
	**Optional**: 
	If you created a Person in Upload documents API, you can skip calling initialize and move to upload document 	API. Alternatively, you can call initialize with personID to attach documents against the person.


.. note:: 
	**OCR API**:
	Response will contain document object with OCR data. For Response look at the end of this document (:doc:`appendex` 2.)

**Path** : /user/person/initialize

**Method** : POST

**Example Request**
 	.. code::
		
		curl -X POST \
		  https://api-dev.springscan.springverify.com/user/person/initialize \
		  -H 'Content-Type: application/json' \
		  -H 'Postman-Token: a251d906-ee0c-4bb7-9f71-1809c1953cc2' \
		  -H 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		  -H 'cache-control: no-cache' \
		  -d '{
		    "selfie": "<selfie_url>",
		    "docType": "ind_pan",
		    "document1": "<document_front_url>",
			"document2": "<optional_back_url>",
		}'


**Query Parameters**
	
  * docType can be: ind_pan, ind_voter_id, ind_driving_license, ind_aadhaar, ind_passport, ind_gst_certificate
  * document1: Url of document
  * document2: (optional) back url of document
  * selfie: selfie of person
  * Header: Client Token and Auth Token
  * personId: person id.

Add/Update Document For Person
------------------------------

Adds a new document to person or updates an existing document.

.. note::
	 Please give the image url in this API.
	 Use the token which was returned after add candidate API.

**Currenly Supported Docs**
	
	* Salary Slip
	* Experience Letter
	* Relieving Letter
	* Appointment Letter
	* Others (not specific doc)

**Path** : /user/person/:personId/document

**Method** : POST

**Example Request**
 	.. code::
		
		 curl -X POST \
		  https://api-dev.springscan.springverify.com/user/person/5df35fa819bd2a8d8663371c/document \
		  -H 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3RAc3ByaW5nc2Nhbi5jb20iLCJ1c2VySWQiOiI1ZGY4OGZjMTllZjFjODM0ODQwOTBmYjAiLCJpYXQiOjE1NzY2NjQ1MzQsImV4cCI6MTU4NTMwNDUzNH0.H-FiqMXSqQkE2gvvrJbCDQU8NQWx1Ru3_Ofk-HHxekM' \	
		  -H 'Postman-Token: 7ca2a5cf-3ee3-49be-8cda-ff8cb475e1f5' \
		  -H 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		  -H 'cache-control: no-cache' \
		  -d '{
			"docType" = "ind_gst_certificate",
			"document1" = "https://springverify-assets-id.s3.amazonaws.com/373/addressDoc-front"	
		    }'

**Query Parameters**
	
  * document1: Url of document
  * document2 (optional): back url of document
  * docType: Can beind_pan, ind_voter_id, ind_driving_license, ind_aadhaar, ind_passport, ind_gst_certificate

Selfie Quality Detection
----------------

Returns quality of selfie image

**Path** : /face/checkQuality

**Method** : POST

**Example Request**
 	.. code::
		
		curl --location --request POST 'https://api-dev.springscan.springverify.com/face/checkQuality' \
		--header 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3RAc3ByaW5nc2Nhbi5jb20iLCJ1c2VySWQiOiI1ZTMwN2IwNGNkNWQ5YTAzMTgwYzMwYWMiLCJpYXQiOjE1ODYzNDU0ODUsImV4cCI6MTU5NDk4NTQ4NX0.7WOKNdv-wZ21cYVKuE8tMF2waecvC1NGUqtyV9pDjKE' \
		--header 'Content-Type: application/json' \
		--data-raw '{
			"selfie_url": "<image_url>",
			"person_id": "<if_generated_earlier>"
		}'

**Query Parameters**
	* selfie_url: Hosting url or Base64 of selfie image
	* person_id: optional, if provided , selfie quality will be stored against the person. else not.
	* replace: optional, attaches the sent selfie url with the person . default is true.

**Response Parameters**
	* face_box : box dimensions
	* face_coverage: contains a message comment about selfie with percentage and status
	* face_detected: boolean for face detection
	* is_live: boolean for liveliness detection
	* multiple_faces_detected: boolean for multiple faces detection
	* person_id: created or returned person's id
	* is_updated_for_user: if true, sent selfie was successfully validated and attached to the user. if false, either selfie validation failed or replace was false in query.


Add/Update Selfie For Person
----------------------------

Adds a new Selfie to person or updates an existing Selfie.

**Path** : /user/person/:personId/selfie

**Method** : POST

**Example Request**
 	.. code::
		
		curl -X POST \
		  https://api-dev.springscan.springverify.com/user/person/5ddcfd3582a9b7001d997e7b/selfie \
		  -H 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InNvdXJhYmguYmFncmVjaGExMjM0NTZAZ21haWwuY29tIiwidXNlcklkIjoiNWNkNDE4MmUzZDhlYWM1NDVjMWMxMWM2IiwiaWF0IjoxNTU3NzI4NDc4LCJleHAiOjE1NTc3NzE2Nzh9.5nQ-wzQOeDqSon_kGg9fqeLtywNSZWUjxonVg75-ndg' \
		  -H 'Content-Type: application/x-www-form-urlencoded' \
		  -H 'Postman-Token: d737d790-e09e-404e-b629-55094d0ea7e7' \
		  -H 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		  -H 'cache-control: no-cache' \
		  -d 'selfieurl=https%3A%2F%2Fpdf-reports-springrole.s3.amazonaws.com%2Fme.jpg'

**Query Parameters**
	
	* selfieUrl: Url of selfie
	* Header: Client Token and Auth Token

Compare Documentation And Selfie
--------------------------------

Does a compare of document and selfie, for a match. If User document image and user selfie matches, generates a high score with a boolean value of true, else false.

**Path** : /user/person/:personId/compare-selfie-and-document

**Method** : POST

**Example Request**
 	.. code::
		
		curl -X POST \
		  https://api-dev.springscan.springverify.com/user/person/5ddcfd3582a9b7001d997e7b/compare-selfie-and-document \
		  -H 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InNvdXJhYmguYmFncmVjaGExMjM0NTZAZ21haWwuY29tIiwidXNlcklkIjoiNWNkNDE4MmUzZDhlYWM1NDVjMWMxMWM2IiwiaWF0IjoxNTU3NzI4NDc4LCJleHAiOjE1NTc3NzE2Nzh9.5nQ-wzQOeDqSon_kGg9fqeLtywNSZWUjxonVg75-ndg' \
		  -H 'Content-Type: application/x-www-form-urlencoded' \
		  -H 'Postman-Token: 8f980d37-444b-4154-bbde-9bc086a39ded' \
		  -H 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		  -H 'cache-control: no-cache' \
		  -d 'docType=ind_driving_license'

**Query Parameters**
	
	* docType :ind_pan, ind_voter_id, ind_driving_license, ind_aadhaar, ind_passport
	* Header: Client Token and Auth Token


Government Verification
-----------------------

Initiates government verification

**Path** : /v2/user/person/governmentCheck/:docType/:personId

**Method** : POST

.. note::
	 For responses look at :doc:`appendex` 1

**Query Parameters**
	
	* Header: Client Token and Auth Token

Government Verification (without ocr)
-------------------------------------

Initiates government verification on id number, name and date of birth or on gstin and legal name provided by client. No OCR is required for this, you can skip ocr step. Ideal if you have IDs and other information in text format.

**Path** : /v2/user/person/governmentCheckDirect

**Method** : POST


.. note::
 	 PersonId is optional. If sent, it will retrieve the existing person. If omitted, api will create and return a new person.

**Query Parameters**

**Driving License**

.. code::
		
		{
			"personId": ":personId",
			"doc_type": "ind_driving_license",
			"date_of_birth": "1993-08-25",
			"name_on_card": "HARISREE HO",
			"id_number": "18/6173/2016"
		}

**Voter ID**

.. code::
		
		{ 
			"personId": ":personId",
			"doc_type": "ind_voter_id",  
			"name_on_card": "HARISREE HO", 
			"id_number": "GDN0225185" 
		} 

**PAN**

.. code::
		
		{ 
			"personId": ":personId",
			"doc_type": "ind_pan",  
			"date_of_birth": "24-08-1991", 
			"name_on_card": "Karan Ahuja",
			"id_number": "BILPA4762R" 
		} 

**AADHAAR**

.. code::
		
		{
			"personId": ":personId",
			"doc_type": "ind_aadhaar",
			"id_number": "475260511399" 
		}

**GST CERTIFICATE**

.. code::
		
		{
			"personId": ":personId",
			"doc_type": "ind_aadhaar",
			"gstin": "29AAYCS8889G1ZZ",
			"legal_name" : "SPRINGROLE INDIA PRIVATE LIMITED" 
		}		

.. note::
   date format is yyyy-mm-dd
   For response check :doc:`appendex` 1
   as this does not go through complete ocr, matched information will be limited to data provided


Court Check API
---------------

Fetches the court case reports matching the name,fatherName and address

**Path** : /criminal/searchDirect

**Method** : POST

**Example Request**
    .. code::

		curl -X POST \
		  https://api-dev.springscan.springverify.com/criminal/searchDirect \
		  -H 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InNvdXJhYmhiYWdyZWNoYTFAZ21haWwuY29tIiwidXNlcklkIjoiNWNkYmFjMTQ4ODY1NzQ0YTIwNGQ1NTA2IiwiaWF0IjoxNTc5Njg4MDA5LCJleHAiOjE1ODgzMjgwMDl9.E0NZd0wa36uKFZtqI0lkxg7rzVWAftTGAQ__Z-bhAb8' \
		  -H 'Postman-Token: 8fd4fb50-9812-43a1-80dd-19a87363aae9' \
		  -H 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		  -H 'cache-control: no-cache' \
		  -d '{
			"name" = "Piyush",
			"fatherName" = "Sanjay",
			"address" = "897h9h7977997"	
		    }'

.. note::
	For Response check :doc:`appendex`	2	

**Query Parameters**
	
	* Name
	* Father's Name
	* Address
	* Header: Client Token and Auth Token



Fetch Person API
----------------

Fetches a person information

**Path** : /user/person/:personId

**Method** : POST

**Example Request**
 	.. code::
		
		 curl -X GET \
		  https://api-dev.springscan.springverify.com/user/person/5df9fdf971b57d2c188ebc62 \
		  -H 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3RAc3ByaW5nc2Nhbi5jb20iLCJ1c2VySWQiOiI1ZGY4OGZjMTllZjFjODM0ODQwOTBmYjAiLCJpYXQiOjE1NzY2NjQ1MzQsImV4cCI6MTU4NTMwNDUzNH0.H-FiqMXSqQkE2gvvrJbCDQU8NQWx1Ru3_Ofk-HHxekM' \
		  -H 'Postman-Token: 8fd4fb50-9812-43a1-80dd-19a87363aae9' \
		  -H 'Token: 4cbe51cf-a294-35a8-b3ae-d3cc89abf29c' \
		  -H 'cache-control: no-cache'

.. note::
	For Response check :doc:`appendex` 2

**Query Parameters**
	
	* Header: Client Token and Auth Token

Aadhaar Masking 
----------------

Masks an Aadhaar image to hide first 12 digits of Aadhaar ID number

**Path** : /verification/maskAadhaar

**Method** : POST

**Example Request**
 	.. code::
		
		curl --location --request POST 'api-dev.springscan.springverify.com/verification/maskAadhaar' \
		--header 'Token: 00ffc975-eafa-4451-9a71-aad62623c963' \
		--header 'Content-Type: application/json' \
		--data-raw '{
			"aadhaar_url": [
				"<aadhar_url_1>",
				"<aadhar_url_2>"],
			"consent": true
			}'

**Query Parameters**
	
	* aadhaar_url: can be an array of aadhaar urls or a single url
	* consent: we will go ahead with masking only when consent is true from you