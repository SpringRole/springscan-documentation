Introduction
============

We provide API access to clients for document OCR and Government verification. You are requested to integrate in our Test Mode first, and test the integration, before shifting to Live Mode.

Defining internal objects
-------------------------

	=============== ============================================
	 ERROR CASES   	 RESPONSE
	=============== ============================================ 
	 **person**  					* We define *person* as an entity on our side, which is used to track/upload/verify document 									 against.
	 		             	
	 **document** 				* We define *document* as an entity to be verified/OCR ed.

	 **User**							* We define *User* as an entity having group of people.

	 **Company**					* We define *Company* as  an entity having group of users.
	=============== ============================================

Document Types Supported are
----------------------------

	.. list-table::
	   :widths: 25 25 25 25
	   :header-rows: 1

	   * - Document
	     - Key
	     - OCR
	     - Verification
	   * - PAN
	     - ind_pan
	     - Yes
	     - Yes
	   * - Voter ID
	     - ind_voter_id
	     - Yes
	     - Yes
	   * - Aadhaar
	     - ind_adhaar
	     - Partial
	     - Yes
	   * - Passport
	     - ind_passport
	     - Yes
	     - No
	   * - Driving License
	     - ind_driving_license
	     - Yes
	     - Yes
	   * - GST Certificate
	     - ind_gst_certificate
	     - Yes
	     - Yes 

Environment Urls
----------------

	**Development** : https://api-dev.springscan.springverify.com

	**Credentials** : 
			* email: <contact us for your test credentials>
			* password: <contact us for your test credentials>


	**Production** :  https://api.springscan.springverify.com


.. note::
	 Contact karan.ahuja@springrole.com for client Token, if you don't already have one.