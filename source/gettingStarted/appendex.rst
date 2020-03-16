Appendex
========

Appendex 1
----------
Understanding Government Responses

Driving License:
****************

**success Response**

.. code::
	  
			{
			    "result": "id_found",
			    "message": "Id was found in the source",
			    "success": true,
			    "ocr": {
			        "address": "M-150, BLK-I NAGAR, PASCHIM VIHAR,DELHI GURUHARKISHAN",
			        "date_of_birth": "1991-08-24",
			        "date_of_validity": null,
			        "fathers_name": "SANJAY AHUJADOB",
			        "id_number": "DL-0420150346015",
			        "is_scanned": "false",
			        "issue_dates": {
			            "LMV": null,
			            "MCWG": null,
			            "TRANS": null
			        },
			        "name_on_card": "KARAN AHUJA",
			        "pincode": "110087",
			        "state": "Delhi",
			        "street_address": "BLK-I NAGAR, PASCHIM VIHAR, GURUHARKISHAN",
			        "type": [
			            "LMV-NT",
			            "MCWG"
			        ],
			        "validity": {
			            "NT": "2035-01-30",
			            "T": null
			        }
			    },
			    "matched_information": {
			        "message": "OCR Data has been verified with government source",
			        "source": "SARATHI",
			        "dl_status": "Active",
			        "status": "id_found",
			        "name_match": 98.33333333333333,
			        "dob_match": true,
			        "ocr_id_match": true
			    }
			}

**dl_status** is status of the Driving License found with source, look for Active/Inactive.

**ocr_id_match** will be true if OCR scanned ID and Government pulled ID were same.

**name_match** will be percentage match  of scanned Name and government retrieved name.

**dob_match** will bebe true if OCR scanned date of birth and Government pulled date of birth were same.

PAN CARD
********

**success response**

.. code::

				{
				    "result": "id_found",
				    "message": "PAN is Active and the details are matching with PAN database.",
				    "success": true,
				    "ocr": {
				        "age": 28,
				        "date_of_birth": "1991-08-24",
				        "date_of_issue": null,
				        "fathers_name": "Sanjay Kumar Ahuja",
				        "id_number": "BILPA4762R",
				        "is_scanned": false,
				        "minor": false,
				        "name_on_card": "Karan Arilia",
				        "pan_type": "Individual"
				    },
				    "matched_information": {
				        "message": "PAN format is correct and PAN number is correct matching against DOB. However, Name is Incorrect.",
				        "id_match": true,
				        "name_match": false,
				        "dob_match": true
				    }
				}

**id_match** if id ocr and govt matched.

**name_match** if name ocr and govt matched.

**dob_match** if date of birth ocr and govt matched.

Voter ID
********

**success response**

.. code::
	  
	  {
		    "result": "id_found",
		    "message": "Id was found in the source",
		    "success": true,
		    "ocr": {
		        "address": "150, BLOCK- M, GURU HAR KISHAN NAGAR PASCHIM VIHAR, DELHI",
		        "age": null,
		        "date_of_birth": null,
		        "district": "DELHI",
		        "fathers_name": "Sanjay Kumar Ahuja",
		        "gender": "MALE",
		        "house_number": "150",
		        "id_number": "UBF2101764",
		        "is_scanned": null,
		        "name_on_card": "Karan Ahuja",
		        "pincode": null,
		        "state": "Delhi",
		        "street_address": "Block- M, Guru Har Kishan Nagar Paschim Vihar, Delhi",
		        "year_of_birth": null
		        },
		    "matched_information": {
		        "message": "OCR Data has been verified with government source",
		        "gender": "M",
		        "source": "NVSP",
		        "status": "id_found",
		        "name_match": 100,
		        "father_name_match": 100,
		        "street_address_match": 64.57571524439514,
		        "ocr_id_match": true
		    }
	  }

**gender** will be Government retrieved gender of person.

**name_match** will be percentage match  of scanned Name and government retrieved name.

**father_name_match** will be percentage match of scanned Name (father/husband or guardian) and government retrieved name.

**street_address_match** will be percentage match  of scanned address and government retrieved address. closer it is to 100, better result. Will rarely be 100.

Aadhaar
*******

**success response**

.. code::
		
	  {
	    "result": "id_found",
	    "message": "found and verified by UIDAI portal",
	    "success": true,
	    "information": "{\"Gender\": \"MALE\", \"State\": \"Delhi\", \"Mobile Number\": \"xxxxxxx447\", \"Age Band\": \"20-30\"}",
	    "ocr": {
	        "address": "S/O Sanjay Ahuja, House No-M 150, Guru karkishan Nagar, Paschim Vihar, Jwala Puri, We st Delhi, Delhi - 110087",
	        "date_of_birth": "1991-08-24",
	        "district": "DELHI",
	        "fathers_name": "Sanjay Ahuja",
	        "gender": "MALE",
	        "house_number": "M 150",
	        "id_number": "319*4429*458",
	        "is_scanned": "false",
	        "name_on_card": "Karan Ahuja",
	        "pincode": "110087",
	        "state": "Delhi",
	        "street_address": "Guru karkishan Nagar, Paschim Vihar, Jwala Puri, We st",
	        "year_of_birth": "1991"
	    },
	    "matched_information": {
	        "message": "OCR Data has been verified with government source",
	        "gender_match": true,
	        "state_match": true,
	        "age_match": true
	    }
	  }

**gender_match** will be true if gender from ocr and goverment are same.

**state_match** will be true if state from ocr and goverment are same.

**age_match** will be true if age from ocr and goverment are same.

GST Certficate:
****************

**success Response**

.. code::
	  
		{
		"idfyResponse": {
			"action": "extract",
			"completed_at": "2020-03-16T19:05:23+05:30",
			"created_at": "2020-03-16T19:05:13+05:30",
			"group_id": "5e6f808f7182b549d2b49223",
			"request_id": "eb2aa363-b732-4d5d-937a-a0317656089d",
			"result": {
				"extraction_output": {
					"address": "FIRST AND FOURTH FLOOR, NO 20, LAKSHMI PLAZA, KRISHNANAGAR INDUSTRIAL LAYOUT, HOSUR ROAD,",
					"constitution_of_business": "Private Limited Company",
					"date_of_liability": "2017-07-24",
					"gstin": "29AAYCS8889G1ZZ",
					"is_provisional": false,
					"legal_name": "SPRINGROLE INDIA PRIVATE LIMITED",
					"pan_number": "AAYCS8889G",
					"trade_name": "",
					"type_of_registration": "Regular",
					"valid_upto": "2017-07-24"
				}
			},
			"status": "completed",
			"task_id": "5e6f808f7182b549d2b49223_1584365711890",
			"type": "ind_gst_certificate",
			"docId": "5e6f809b7182b549d2b49224"
		},
		"personId": "5e6f808f7182b549d2b49223"
		}


Appendex 2
----------

**success response**

.. code::
		
	{  "person": 
	    {
	        "name": {
	            "first": "Karan",
	            "last": "Ahuja",
	            "middle": "Ahuja"
	        },
	        "documents": {
	          "ind_aadhaar": {
	            "result": {
	              "address": "S/O Sanjay Ahuja, House No-M 150, Guru karkishan Nagar, Paschim Vihar, Jwala Puri, We st Delhi, Delhi - 110087",
	              "date_of_birth": "1991-08-24",
	              "district": "DELHI",
	              "fathers_name": "Sanjay Ahuja",
	              "gender": "MALE",
	              "house_number": "M 150",
	              "id_number": "319644293458",
	              "is_scanned": "false",
	              "name_on_card": "Karan Ahuja",
	              "pincode": "110087",
	              "state": "Delhi",
	              "street_address": "Guru karkishan Nagar, Paschim Vihar, Jwala Puri, We st",
	              "year_of_birth": "1991"
	            },
	              "manualObj": null,
	              "status": "completed",
	              "faceMatched": false,
	              "matchResult": null,
	              "govResult": null,
	              "request_id": "1b247fa9-df84-463e-aa3f-899758ab6019",
	              "provider": "idfy",
	              "_id": "5df9fdfb71b57d2c188ebc63",
	              "docType": "ind_aadhaar",
	              "document1": "https://pdf-reports-springrole.s3.amazonaws.com/adhaar.png",
	              "belongsTo": "5df9fdf971b57d2c188ebc62",
	              "createdAt": "2019-12-18T10:22:59.917Z",
	              "updatedAt": "2019-12-18T10:23:01.167Z",
	              "__v": 0
	            },
	            "ind_driving_license": null,
	            "ind_pan": null,
	            "ind_voter_id": null,
	            "ind_passport": null
	        },
	        "selfie": {
	            "url": "https://pdf-reports-springrole.s3.amazonaws.com/face_image_1573552012776.jpg"
	        },
	        "hasConsent": false,
	        "phone": null,
	        "city": null,
	        "gender": null,
	        "s3_paths": null,
	        "_id": "5df9fdf971b57d2c188ebc62",
	        "addedBy": "5df88fc19ef1c83484090fb0",
	        "createdAt": "2019-12-18T10:22:49.563Z",
	        "updatedAt": "2019-12-18T10:23:00.299Z",
	        "__v": 0
	    }
	}

**Person** object will contain name and document objects

**document** object will contain one of the 5 supported document type (table in beginning of this document.

**result** object inside ind_*  object is the ==OCR result==

**govResult** is government result object, filled after government verification (5) api is called

**document1** is the link of document

Court Check
***********

**success response**

.. code::
		
	{
      "reports": [
         {
            "year": "2017",
            "subject": null,
            "address_taluka": null,
            "source": "ecourt",
            "type": 1,
            "next_hearing_date": " 21st December 2017",
            "address_pincode": null,
            "first_hearing_date": " 28th November 2017",
            "state_name": "Haryana",
            "address_wc": 0,
            "id": null,
            "under_acts": "Motor Vehicles Act",
            "address_district": null,
            "nature_of_disposal": null,
            "uniq_case_id": "e62aad327db4ec520d7312ad660ab851",
            "name_wc": 5,
            "business_category": "Motor Vehicles",
            "filing_no": null,
            "case_category": "criminal",
            "address_street": null,
            "name": "Ayush s o Sanjay Singla",
            "dist_code": 7,
            "state_code": 14,
            "link": "https://pdf-reports-springrole.s3.amazonaws.com/governmentReport/0.698914320380329",
            "address_state": null,
            "court_no_judge": null,
            "decision_date": null,
            "court_no_name": null,
            "under_sections": "53",
            "court_name": null,
            "case_no_year": null,
            "address": null,
            "case_code": "204100086582017",
            "dist_name": "Hisar",
            "case_type": "Pending",
            "police_station": "Traffic",
            "case_year": "2017",
            "registration_no": null,
            "case_decision_date": null,
            "purpose_of_hearing": " Appereance",
            "case_status": null,
            "fir_no": "0              ",
            "md5": "96baa5ada5caaf925769af05596556ce",
            "raw_address": null,
            "court_code": 4,
            "cnr": "HRHS020162142017",
            "data_category": " The_Motor_Vehicles_Act__1988 The_Delhi_Motor_Vehicles_Taxation_Act__1962 53",
            "global_category": "motor police",
            "oparty": "State of Haryana",
            "score": 72.58,
            "model_score": -4.394297
        },
        {
            "year": "2018",
            "subject": null,
            "address_taluka": null,
            "source": "ecourt",
            "type": 1,
            "next_hearing_date": " 06th June 2018",
            "address_pincode": null,
            "first_hearing_date": " 02nd April 2018",
            "state_name": "Bihar",
            "address_wc": 0,
            "id": null,
            "under_acts": "Indian Penal Code",
            "address_district": null,
            "nature_of_disposal": null,
            "uniq_case_id": "760d3f8a839b02c327cbda809c96d338",
            "name_wc": 5,
            "business_category": "Serious",
            "filing_no": null,
            "case_category": "criminal",
            "address_street": null,
            "name": "AAYUSH URF RANJAY KUMAR RAM",
            "dist_code": 6,
            "state_code": 8,
            "link": "https://pdf-reports-springrole.s3.amazonaws.com/governmentReport/0.7151153518381306",
            "address_state": null,
            "court_no_judge": null,
            "decision_date": null,
            "court_no_name": null,
            "under_sections": "323,504,457,379,354B,34",
            "court_name": null,
            "case_no_year": null,
            "address": null,
            "case_code": "214200003962018",
            "dist_name": "Begusarai",
            "case_type": "Pending",
            "police_station": null,
            "case_year": "2018",
            "registration_no": null,
            "case_decision_date": null,
            "purpose_of_hearing": " Soleman Affirmation (S.A)",
            "case_status": null,
            "fir_no": null,
            "md5": "36675bbbfc841e7e9f89694e5a96413f",
            "raw_address": null,
            "court_code": 3,
            "cnr": "BRBE020016252018",
            "data_category": "imprisonment fine The_Indian_Penal_Code__1860 323 504 457 379 354 34 354B",
            "global_category": "ability ipap police",
            "oparty": "MAMTA DEVI",
            "score": 72.58,
            "model_score": -4.394297,
            "imprisonment": "Possibility of imprisonment upto a maximum of 23 years",
            "fine": "Possibility of fine upto to a maximim of Rupees 1000"
        },
        {
            "year": "2018",
            "subject": null,
            "address_taluka": null,
            "source": "ecourt",
            "type": 1,
            "next_hearing_date": null,
            "address_pincode": null,
            "first_hearing_date": " 29th March 2018",
            "state_name": "Haryana",
            "address_wc": 0,
            "id": null,
            "under_acts": "Motor Vehicles Act",
            "address_district": null,
            "nature_of_disposal": " Uncontested--CONFESSION",
            "uniq_case_id": "40ca51a88d0a629b4cd520ea19c977b4",
            "name_wc": 5,
            "business_category": "Motor Vehicles",
            "filing_no": null,
            "case_category": "criminal",
            "address_street": null,
            "name": "Ayush S o Sh  Snajay",
            "dist_code": 12,
            "state_code": 14,
            "link": "https://pdf-reports-springrole.s3.amazonaws.com/governmentReport/0.584659322133976",
            "address_state": null,
            "court_no_judge": null,
            "decision_date": " 03rd April 2018",
            "court_no_name": null,
            "under_sections": "53",
            "court_name": null,
            "case_no_year": null,
            "address": null,
            "case_code": "204200016792018",
            "dist_name": "Rohtak",
            "case_type": "Disposed",
            "police_station": null,
            "case_year": "2018",
            "registration_no": null,
            "case_decision_date": null,
            "purpose_of_hearing": null,
            "case_status": " CASE DISPOSED",
            "fir_no": null,
            "md5": "b4b72ce60c48a823377fd4e12f4af211",
            "raw_address": null,
            "court_code": 4,
            "cnr": "HRRH030021752018",
            "data_category": " The_Motor_Vehicles_Act__1988 The_Delhi_Motor_Vehicles_Taxation_Act__1962 53",
            "global_category": "motor",
            "oparty": "State",
            "score": 72.58,
            "model_score": -4.394297
        },
        {
            "year": "",
            "subject": "",
            "link": "https://pdf-reports-springrole.s3.amazonaws.com/governmentReport/d8e6bd1d9fbb9326263e791d21f9109c",
            "court_no_judge": "2-Jt.Civil JudgeJr. Dn.  JMFC. Tirora",
            "source": "ecourt",
            "type": 0,
            "next_hearing_date": "26th February 2019",
            "decision_date": null,
            "first_hearing_date": "22nd February 2019",
            "state_name": "MAHARASHTRA",
            "court_no_name": "",
            "under_sections": "12",
            "address_wc": 1,
            "id": "d8e6bd1d9fbb9326263e791d21f9109c",
            "under_acts": "Protection of Women from Domestic Violence Act",
            "court_name": "Civil Court Junior Division , Tirora",
            "nature_of_disposal": null,
            "case_no_year": "",
            "uniq_case_id": "d8e6bd1d9fbb9326263e791d21f9109c",
            "name_wc": 3,
            "business_category": "Serious",
            "address": "Satona",
            "case_code": "209700000042019",
            "time_stamp": "2019-02-27T00:00:00Z",
            "dist_name": "GONDIA",
            "case_type": "PWDVA Appln. - Application under Domestic Violence Act",
            "police_station": "",
            "filing_no": "217/2019      22-02-2019  ",
            "case_year": "2019",
            "registration_no": "4/2019    22-02-2019",
            "case_decision_date": "",
            "purpose_of_hearing": "Awaiting Notice",
            "case_category": "criminal",
            "case_status": null,
            "name": "Ayush Sanjay Shende",
            "dist_code": 11,
            "fir_no": "",
            "state_code": 1,
            "md5": "08f95e3cd897589ef61aff4947f34834_4d99972aa897f4aa161ffb927a2f18b3",
            "raw_address": "    Satona",
            "court_code": 6,
            "cnr": "MHGO080002332019",
            "data_category": " The_Protection_of_Women_from_Domestic_Violence_Act__2005 12",
            "global_category": "",
            "fhd": "2019-02-22",
            "oparty": "Taramati Rameshwar Shende, Rameshwar Madho Shende, Sanjay Rameshwar Shende 3, Munnibai Dilip Tumsare",
            "score": 68.91,
            "model_score": -5.0140433
        },
        {
            "year": " 0",
            "subject": "",
            "link": "https://pdf-reports-springrole.s3.amazonaws.com/governmentReport/59565d294962f2ad924daf16ae98e952",
            "court_no_judge": " 18-Judicial Magistrate -  Ist Class",
            "source": "ecourt",
            "type": 1,
            "next_hearing_date": " 14th November 2018",
            "decision_date": null,
            "first_hearing_date": " 03rd July 2018",
            "state_name": "HARYANA",
            "court_no_name": "",
            "under_sections": "",
            "address_wc": 0,
            "id": "59565d294962f2ad924daf16ae98e952",
            "under_acts": "",
            "court_name": "Chief Judicial Magistrate, Hisar",
            "nature_of_disposal": null,
            "case_no_year": "",
            "uniq_case_id": "59565d294962f2ad924daf16ae98e952",
            "name_wc": 4,
            "business_category": "Miscellaneous",
            "address": "",
            "case_code": "204100047392018",
            "time_stamp": "2018-09-09T00:00:00Z",
            "dist_name": "HISAR",
            "case_type": " SUMM",
            "police_station": " Traffic",
            "filing_no": " 9660/2018    03-07-2018",
            "case_year": "2018",
            "registration_no": " 4739/2018     03-07-2018",
            "case_decision_date": "",
            "purpose_of_hearing": " Appereance",
            "case_category": "criminal",
            "case_status": null,
            "name": "Aayush s o Sanjay",
            "dist_code": 7,
            "fir_no": " 0",
            "state_code": 14,
            "md5": "9bf659af06821b054240c50db8abcb8b_c579ba08cfa342173bea3f2c6959849f",
            "raw_address": "",
            "court_code": 4,
            "cnr": "HRHS020096722018",
            "data_category": "  ",
            "global_category": "police",
            "oparty": "State of Haryana",
            "score": 64.18,
            "model_score": -5.759428
        },
        {
            "year": "2017",
            "subject": null,
            "address_taluka": null,
            "source": "ecourt",
            "type": 0,
            "next_hearing_date": null,
            "address_pincode": null,
            "first_hearing_date": " 11th October 2017",
            "state_name": "Bihar",
            "address_wc": 0,
            "id": null,
            "under_acts": "Hindu Marriage Act",
            "address_district": null,
            "nature_of_disposal": " Uncontested--ALLOWED",
            "uniq_case_id": "13ef7eacb5d8a5b6434881ae2ab1017a",
            "name_wc": 4,
            "business_category": "",
            "filing_no": null,
            "case_category": "civil",
            "address_street": null,
            "name": "Ayush Kumar   Sanjay Kumar",
            "dist_code": 28,
            "state_code": 8,
            "link": "https://pdf-reports-springrole.s3.amazonaws.com/governmentReport/0.6544573942723126",
            "address_state": null,
            "court_no_judge": null,
            "decision_date": " 22nd November 2017",
            "court_no_name": null,
            "under_sections": "13B",
            "court_name": null,
            "case_no_year": null,
            "address": null,
            "case_code": "217500001442017",
            "dist_name": "Bettiah",
            "case_type": "Disposed",
            "police_station": null,
            "case_year": "2017",
            "registration_no": null,
            "case_decision_date": null,
            "purpose_of_hearing": null,
            "case_status": " CASE DISPOSED",
            "fir_no": null,
            "md5": "f5d19b4e73fd675793d8ed13b08e0cc3",
            "raw_address": null,
            "court_code": 2,
            "cnr": "BRWC010105242017",
            "data_category": " The_Hindu_Marriage_Act__1955 The_Hindu_Marriage__Validation_of_Proceedings__Act__1960 13",
            "global_category": "",
            "oparty": "Shivani Kumari   Sudha",
            "score": 64.18,
            "model_score": -5.759428
        	}
		],
		"status": "completed",
		"_id": "5e6f883229155a001d00a8f4",
		"belongsTo": "5e6f882629155a001d00a8f3",
		"query": {
			"name": "Piyush",
			"address": "897h9h7977997",
			"fatherName": "Sanjay "
		},
		"createdAt": "2020-03-16T14:07:46.285Z",
		"updatedAt": "2020-03-16T14:07:46.285Z",
		"__v": 0
	}