Appendex
========

Appendex 1
----------
Understanding Government Responses

Driving License:
****************

**success Response**

**OCR**

.. code-block:: json
	  
					{
						"got_face_match": true,
						"got_ocr_response": true,
						"got_gov_response": true,
						"result": "id_found",
						"message": "Id was found in the source",
						"success": true,
						"ocr": {
							"address": "M-150, BLK-I NAGAR, PASCHIM VIHAR,DELHI GURUHARKISHAN",
							"date_of_birth": "1991-08-24",
							"date_of_validity": null,
							"fathers_name": "SANJAY AHUJA",
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
						"government_output": {
							"id_number": "DL04 20150346015",
							"name": "KARAN  AHUJA",
							"dob": "1991-08-24",
							"gender": "M",
							"blood_group": "U",
							"citizenship": "IND",
							"relatives_name": "SANJAY  AHUJA",
							"permanent_address": "M-150,   BLK-M    GURUHARKISHAN NAGAR,PASCHIM  VIHAR,DELHI",
							"temporary_address": "M-150,   BLK-M    GURUHARKISHAN NAGAR,PASCHIM  VIHAR,DELHI",
							"state": "DL",
							"city": null,
							"has_face_image": true,
							"face_image": "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",
							"dl_status": null,
							"issuing_rto_name": "DY.DIR.ZONAL OFFICE,WEST DELHI,JANAKPURI",
							"date_of_issue": "2015-01-31",
							"transport_date_of_issue": "1900-01-01",
							"transport_date_of_expiry": "1900-01-01",
							"cov_details": [
								"MCWG  ",
								"LMV   "
							],
							"cov_issue_date": null,
							"hazardous_valid_till": null,
							"hill_valid_till": null,
							"date_of_last_transaction": null,
							"nt_validity_from": null,
							"nt_validity_to": null,
							"t_validity_from": null,
							"t_validity_to": null,
							"badge_details": null,
							"card_serial_no": null
						},
						"face_match_output": {
							"match_score": 82.66,
							"face_match": true
						},
						"matched_information": {
							"message": "OCR Data has been verified with government source",
							"gender": "M",
							"dl_status": "active",
							"status": "id_found",
							"name_match": 100,
							"dob_match": true,
							"father_name_match": 100,
							"street_address_match": 91.04835651074589,
							"ocr_id_match": true,
							"state_match": true
						}
					}

**dl_status** is status of the Driving License found with source, look for Active/Inactive.

**ocr_id_match** will be true if OCR scanned ID and Government pulled ID were same.

**name_match** will be percentage match  of scanned Name and government retrieved name.

**dob_match** will be true if OCR scanned date of birth and Government pulled date of birth were same.

**father_name_match** will be percentage match of scanned fathers Name and government retreived Name.

**street_address_match** will be percentage match of scanned address and government retreived address.

**state_match** will be true If scanned state and government retreived state are same.

**NO-OCR**

.. code-block:: json
	  
					{
						"got_gov_response": true,
						"result": "id_found",
						"message": "Id was found in the source",
						"success": true,
						"ocr": {
							"date_of_birth": "1991-08-24",
							"id_number": "DL-0420150346015",
						},
						"government_output": {
							"id_number": "DL04 20150346015",
							"name": "KARAN  AHUJA",
							"dob": "1991-08-24",
							"gender": "M",
							"blood_group": "U",
							"citizenship": "IND",
							"relatives_name": "SANJAY  AHUJA",
							"permanent_address": "M-150,   BLK-M    GURUHARKISHAN NAGAR,PASCHIM  VIHAR,DELHI",
							"temporary_address": "M-150,   BLK-M    GURUHARKISHAN NAGAR,PASCHIM  VIHAR,DELHI",
							"state": "DL",
							"city": null,
							"has_face_image": true,
							"face_image": "/9j/4AAQSkZJRgABAQEAAAAAAAD/2wBDAAgGBgcGBQgHBwcJCQgKDBQNDAsLDBkSEw8UHRofHh0aHBwgJC4nICIsIxwcKDcpLDAxNDQ0Hyc5PTgyPC4zNDL/2wBDAQkJCQwLDBgNDRgyIRwhMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjIyMjL/wAARCAB9AG0DASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwDYHT3pcUzPNJu96+0PnB/Gc0h5FJu460gPNAWuPAz0pGljjYKXUMe2azdS1GSHMEMLFzj5jwv41zmp39xBMyRK6BvvSEfe9cGvFxWZNS5aX3npUcIrXmdpcypBHuBJz04qnFqDn/WomCeNjcj65rjIdau4ozH5rbf7p5FWBqJuSGlZU2jgqMVwvH4i97m7w1NK1jtRf2qy+W8ojbH8fGfxq53rhY75J18ma3DQOCA+M/iK2NC1VI8afK53A4iY9x6V34XMHUnyVDmrYbkV4HS0qNg8io9350/dx616bOUlJBNBxUYYCguc8GpsVexm5opuaN2K6GY2Hg1XuJQskMOP9Y3OTgYFSbu/auZ1XVWGpAxONsGVXA7kcmvOzLEOnS5YvVnZg6XNPmfQuXreW7l53klY9GOAo9AKqXETSJh1DNt4x2pLKOTU2fajHYNzN2Ue5q3bW89yP3a4jHyhsdfpXy7mkeuqbdjKt7e3ScRzIWB4JUU+8sIbdhJE4bpmOQf54rVe08qdFwC/Wuhm0mC6094ZoQzEYDKvIOOoqHWXQ0dGXU8+k1CQCQSW0ZiI+UbcbPcVGbwjZNHlZUOVIPBr0K18MqtikN7GqTmMbmUcZ9xXn1/p0lhqT2bDhWwGHSrp1U5W6kVaVlqehWs6XFvHMjBlYAgg5qwDg9eK5LwrO0c91abyYwBIAexzg11G7PFfXYar7akpnhzhyScSbeKTcKjpC9b2JuUic0Cm7hTS4A5qjMLjP2eQL12nHOO1cOY2nuzEnLFyB7812E8xaJ1XglSAaxPA9qt/420+GV8KGeQg9W2qTivCzh25X6nqZfG6sd94E8MTQaLK+oRYa8OfKbkiPGAD9eTXQ3HhEwYaKQCIfdj2gbfyqp4k8aL4ZuI4Y4BJMwz8xwAK5tvijq87jFnD5YPIJOSK+bs5JtnsqXK+WJvf8I5tmaRowxPGc9q1tP0rDhnRRjpXMW/je4uUYvalWHQA9awtV8Ya7JOVt7kWsSjA2jk/XNRGKuXJ6HpF9b7nPevKfH2ny2d/FfAfuZTs3Ds3Xmq7+IvErc/b3bcMAgAH6iuhvGuNb+H98byTddW6NIxxgnaMjpxWiXJJSTMZPmi1Y5LwuWfVZn3YHlHcP73NdgG9K47woQ17cEMPlQDr3zXWqRX2GXfwEeBiP4jJw2eDRx9Ki3Uu/wBK9CxjYosfeq7uc05n4qJmqWyUrjWfapb0Ga0tI8M3Gj+MNI1Bb2ylV7nZLFA5LRMyNkEY9O/rWUxyMHoa6vSkjbRZdWjjaWeO6gaXaCTHs+8ePXk/jXiZy5+yVtr6nr5bGm+Zt6k3jHwxeajdtqECoYlUBmfPy/gAa4B9PninkWSWFkA+VosnJ7dQK93tb9GgwAro449CKzLvw7ocZa/aBFK/NsVRjNfMxk0j1eVN6nOfD3ww1yt3eX6sIxtSFTx9T/Sub1/Q7i3u5V2llV+CO617Hpoi0/S080xxs3zlAQMZ7VzurCEzrcjZJHuKuFOSB61UtEmtwheTa6Hl2maJJcziCETtLI+BknCD6V6DNokWmeGry0Lly9tIrE+pQitWD7JaxF7dVQkdQOtYHiDUJ5dPmhiGXlHlDnH3jt/rUt30YKNjEt7J9M0iOFAFtJFR0GBncQSTnGSeKj3Z71veLYItMg0ywg3mJI2O9jktjAzn865gSDPWvrsoi1hlfqzwcfJSruxaDGlLVX8wdQaUye9erc5ErFBm4qMsc0HJzUTN3rmcu47dhxatfw34gOgXlzLsaSOaAoYxjBcEbSfwzWEX/KmFq56yjUi4S2ZtRk6UuaJ6zpN1HPpdpcRqFV41O1einHStOGKG4dZL1v3KHOz1PavOfC+urbQtYTuBtO6LJxkE9PzP610t441WOKI3ctrGpyxiO1j6YNfH4in7Kq49j6GlL2kE11GeK9DuftaXmhx3B804khEmFPowUnj/AD0qloNjDpUlxcX4jluJQFZBMrmP1zz16VkasujxnZbxalPMDzcm7JP09P0qna2mnzhR9huIyowW89sn64NTfqb8jtbmOtkuYlBa3cmFjwp7Vi6lcbrZ1bkvxg+lMLrawmKMnZ1G45xWTNdG4JYE+WDtB9TXRgqXtK8UzlxlTkpMGmdlVS7MqDChmJAHt6U0SVGfak6dK+vi+VWWx8/L3tWTiQ0/du71AvXmpMVqpshorse1V34NSMeaic8VlPuOKuRs3ambsc0mcuEUFnPRVGSfwFaVpoF1dTIs4WGLPzhm+Yj0wK4a1aFPWTsdNOjKbskbHhOxhOorDeZJ1CzlURgchPlYH6/LmtCK9TTL0aZqx5z+7n6LIvY+x9RWXaXog+Jeju5CxOZIR6DMbAD88V03iXTItRgaLbvXO5R/Ejeqn+lfM16jqT55dT26ceSPLHoVNS1DSre38q3t42c+tZ1trNkLfa0Ajb88VyE0VxbzGOQuHHUMCM+/NIkMs/AY471Ciu5XNK2xq6lqv2y48m0U/OcA47etM1CUaTfWVpg+S9uchjwx3cn61e0PTooJfPmAbbzz3qLxnpr3VjBrcRP+jyCCRP8AYfof++hj8auElGa5SZwfL7xFPGECuhzG4yp/pUQPFP05S+liKUkEEMDjpT1ti5/cukg9jg/ka+iwmPhKHLUdmeRWwsoyvBaEQb2p4ahoJYsF4mGfaow49a9ONSMvhdzllCSeo+3067u13RRYT++/yitCLQYE5urkyH+5GNo/PrWrPcjGAelZzy5OQa+Zq5lWqO0dF5f5nswwdKGr1J9tvYwOLaJY+Oq9T+NSWYxHCfYsx9zWS85N2IDwCM5rQ02fNqqylVZR8+TgD864JNvVvU6YpLY5vxSZYJ4bmEgTwyCWI/7SnNde+vJd2cF2hwtwgcAnkHuPwOa5zVdV0WcNBLeQyITg+WS2D7EZrd8Evo02lXmn3d1HLZxvvjeUFdu7kjn06596mSvHUcXZszNRuFvtu/kr0NRREKm1VA+grf1XwgYpUm0yXzIJFDKM5BBHBBqjbaJqEkgQ27r6naai5tpa5BbrNPKkECl5GPQdvrXQeIoF07wNNaSKzyXM8ILhflGHDYz+Hrzmur0LQbOxjTzdiSuM4LAFvpWD8QbwTWUWmWoxH9q3uV6YRR1/4Ef/AB2ril1MJzbdkcXaKfJzSsIzJ8y4fqGHGalhUJHtwRVOZmMv0Nax3JLSXbL8u40/zY5OXRCfUqKzGfEhz3oaUrxWmq2dhS10ZotOWIx0IqNWzKRnqKr27Ex4z0OKlPEi49KxtrYt6kM4P26NieegqaSyi1CF7a43CN8Z2nB9jTL0bGt3HXdVlsqgkU4Zf1pK/QLdDg7zT3sbyS1k5KMV6dR2P41JpxTzxDLtzv2kOOCPrXTa1bpdCKdx8/TNZT2kS38bYzvXkVqp8yszFQcHoe0eDL+DUtDt0JXdbZhdRxgD7v6Yrs0t7dBnYteDeEtUuNM8QpbxMWjuRtYE9MDIP+fWvSdY164sPCN7exjMioFX5uhY4zWLjZ3Rc05W1scJ441NNX1qWe3kaNrb9zCVYqCBnJ98nNcDe3NxNPnz5dw6kOR0+lXbqeSRgpboM59aolAE3ZyTW9OKSIk+iIEvb+Ekx3lyvfHmsR+Wa61WlZf3rb3BI3eo7H8q5m3QPMAfWulX77U562CFxkmQ4Pakl+8CO4p0w+UU2XkJ9KT2Gz//2QA=",
							"dl_status": null,
							"issuing_rto_name": "DY.DIR.ZONAL OFFICE,WEST DELHI,JANAKPURI",
							"date_of_issue": "2015-01-31",
							"transport_date_of_issue": "1900-01-01",
							"transport_date_of_expiry": "1900-01-01",
							"cov_details": [
								"MCWG  ",
								"LMV   "
							],
							"cov_issue_date": null,
							"hazardous_valid_till": null,
							"hill_valid_till": null,
							"date_of_last_transaction": null,
							"nt_validity_from": null,
							"nt_validity_to": null,
							"t_validity_from": null,
							"t_validity_to": null,
							"badge_details": null,
							"card_serial_no": null
						},
						"matched_information": {
							"message": "OCR Data has been verified with government source",
							"gender": "M",
							"dl_status": "active",
							"status": "id_found",
							"dob_match": true,
							"ocr_id_match": true
						}
					}

**dl_status** is status of the Driving License found with source, look for Active/Inactive.

**ocr_id_match** will be true if OCR scanned ID and Government pulled ID were same.

**dob_match** will bebe true if OCR scanned date of birth and Government pulled date of birth were same.

PAN CARD
********

**success response**

**OCR**

.. code-block:: json

					  {
						"got_ocr_response": true,
						"got_gov_response": true,
						"result": "id_found",
						"msg": "Pan Details are valid!",
						"message": "PAN is Active and the details are matching with PAN database.",
						"success": true,
						"ocr": {
							"age": 24,
							"date_of_birth": "1996-08-25",
							"date_of_issue": null,
							"fathers_name": "SANJEEV KUMAR",
							"id_number": "HZBPS9811N",
							"id_scanned": false,
							"minor": false,
							"name_on_card": "ANURAG SINDHU",
							"pan_type": "Individual"
						},
						"government_output": {
							"incomeTax": {
								"check": "PAN",
								"dob": "25/08/1996",
								"message": "PAN is Active and the details are matching with PAN database.",
								"name": "ANURAG SINDHU",
								"pan_number": "HZBPS9811N",
								"status": 1,
								"user": "vp_inhouse_docverify"
							},
							"nsdl": {
								"data": {
									"client_id": "pan_dpzjKVcQJPFjmulSWpTj",
									"pan_number": "HZBPS9811N",
									"full_name": "ANURAG SINDHU",
									"category": "person"
								},
								"status_code": 200,
								"success": true,
								"message_code": "success"
							}
						},
						"matched_information": {
							"message": "PAN is Active and the details are matching with PAN database.",
							"id_match": true,
							"name_match": 100,
							"dob_match": true
						}
					  } 

**id_match** if id ocr and govt matched.

**name_match** if name ocr and govt matched.

**dob_match** if date of birth ocr and govt matched.

**NO-OCR**

.. code-block:: json

					  {
						"got_gov_response": true,
						"result": "id_found",
						"msg": "Pan Details are valid!",
						"message": "PAN is Active and the details are matching with PAN database.",
						"success": true,
						"ocr": {
							"id_number": "HZBPS9811N",
        						"date_of_birth": "25-08-1996",
        						"name_on_card": "ANURAG SINDHU"
						},
						"Government_output": {
							"incomeTax": {
								"check": "PAN",
								"dob": "25/08/1996",
								"message": "PAN is Active and the details are matching with PAN database.",
								"name": "ANURAG SINDHU",
								"pan_number": "HZBPS9811N",
								"status": 1,
								"user": "vp_inhouse_docverify"
							},
							"nsdl": {
								"data": {
									"client_id": "pan_dpzjKVcQJPFjmulSWpTj",
									"pan_number": "HZBPS9811N",
									"full_name": "ANURAG SINDHU",
									"category": "person"
								},
								"status_code": 200,
								"success": true,
								"message_code": "success"
							}
						},
						"matched_information": {
							"message": "PAN is Active and the details are matching with PAN database.",
							"id_match": true,
							"name_match": 100,
							"dob_match": true
						}
					  }

**id_match** if id ocr and govt matched.

**name_match** if name ocr and govt matched.

**dob_match** if date of birth ocr and govt matched.

Voter ID
********

**success response**

**OCR**

.. code-block:: json
	  
				{	
					"got_ocr_response": true,
					"got_gov_response": true,
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
					"government_output": {
						"id_number": "UBF2101764",
						"name_on_card": "KARAN  AHUJA",
						"age": "28",
						"dob": null,
						"gender": "M",
						"relation_name": "SANJAY KUMAR  AHUJA",
						"relation_type": "F",
						"house_no": "150",
						"district": null,
						"state": "NCT OF Delhi",
						"assembly_constituency": "NANGLOI JAT",
						"assembly_constituency_number": null,
						"parliamentary_constituency": null,
						"polling_station": "BOSCO PUBLIC SCHOOL NEAR LAKE VIEW APPARTMENTS, PASCHIM VIHAR",
						"part_name": "NANGLOI JAT",
						"part_number": "110",
						"serial_no": null,
						"polling_date": null
					},	
					"matched_information": {
						"message": "OCR Data has been verified with government source",
						"gender": "M",
						"source": "NVSP",
						"status": "id_found",
						"name_match": 100,
						"gender_match": true,
						"state_match": false,
						"house_no_match": true,
						"father_name_match": 100,
						"street_address_match": 69.57602339181285,
						"ocr_id_match": true
					}
				}

**gender** will be Government retrieved gender of person.

**ocr_id_match** will be true if scanned voterId is same as government retreived voterId.

**gender_match** will be true if scanned gender is same as government retreived gender.

**state_match** will be true if scanned state is same as goverment retrieved state.

**house_no_match** will be true if scanned House Number is same as goverment retrieved House Number.

**name_match** will be percentage match  of scanned Name and government retrieved name.

**father_name_match** will be percentage match of scanned Name (father/husband or guardian) and government retrieved name.

**street_address_match** will be percentage match  of scanned address and government retrieved address. closer it is to 100, better result. Will rarely be 100.

**NO-OCR**

.. code-block:: json
	  
				{	
					"got_ocr_response": true,
					"got_gov_response": true,
					"result": "id_found",
					"message": "Id was found in the source",
					"success": true,
					"ocr": {
						"id_number": "UBF2101764",
						"name_on_card": "KARAN AHUJA"
					},
					"government_output": {
						"id_number": "UBF2101764",
						"name_on_card": "KARAN  AHUJA",
						"age": "28",
						"dob": null,
						"gender": "M",
						"relation_name": "SANJAY KUMAR  AHUJA",
						"relation_type": "F",
						"house_no": "150",
						"district": null,
						"state": "NCT OF Delhi",
						"assembly_constituency": "NANGLOI JAT",
						"assembly_constituency_number": null,
						"parliamentary_constituency": null,
						"polling_station": "BOSCO PUBLIC SCHOOL NEAR LAKE VIEW APPARTMENTS, PASCHIM VIHAR",
						"part_name": "NANGLOI JAT",
						"part_number": "110",
						"serial_no": null,
						"polling_date": null
					},	
					"matched_information": {
						"message": "OCR Data has been verified with government source",
						"gender": "M",
						"source": "NVSP",
						"status": "id_found",
						"name_match": 100,
						"ocr_id_match": true
					}
				}

**name_match** will be percentage match  of scanned Name and government retrieved name.

**ocr_id_match** will be true if scanned voterId is same as government retreived voterId.

Aadhaar
*******

**success response**

**OCR**

.. code-block:: json
		
			 {
				"got_ocr_response": true,
				"got_gov_response": true,
				"result": "id_found",
				"message": "found and verified by UIDAI portal",
				"success": true,
				"information": "{\"Gender\": \"MALE\", \"State\": \"Delhi\", \"Mobile Number\": \"xxxxxxx447\", \"Age Band\": \"20-30\"}",
				"ocr": {
					"id_number": "319644293458",
					"vid_number": null,
					"enrollment_number": null,
					"name_on_card": "Karan Ahuja",
					"date_of_birth": "1991-08-24",
					"year_of_birth": "1991",
					"gender": "MALE",
					"phone_number": null,
					"fathers_name": "Sanjay Ahuja",
					"parents_name": "Sanjay Ahuja",
					"husband_name": null,
					"address": "S/O Sanjay Ahuja, House No-M 150, Guru karkishan Nagar, Paschim Vihar, Jwa la Puri, We st Delhi, Delhi - 110087",
					"house_number": "M 150",
					"street_address": "Guru karkishan Nagar, Paschim Vihar, Jwa la Puri, We st",
					"district": "DELHI",
					"state": "Delhi",
					"pincode": "110087"
				},
				"government_output": {
					"aadhaar_number": "319644293458",
					"Gender": "MALE",
					"State": "Uttarakhand",
					"phone_number": "650",
					"age_band": "20-30"
				},
				"matched_information": {
					"message": "OCR Data has been verified with government source",
					"gender_match": true,
					"state_match": false,
					"age_match": true,
					"id_match": true
				}
			 }

**gender_match** will be true if gender from ocr and government are same.

**state_match** will be true if state from ocr and government are same.

**age_match** will be true if age from ocr and government are same.

**id_match** will be true if aadhaarId from ocr is same as government retrieved aadhaarId.

**NO-OCR**

.. code-block:: json
		
			  {
				"got_gov_response": true,
				"result": "id_found",
				"message": "found and verified by UIDAI portal",
				"success": true,
				"information": "{\"Gender\": \"MALE\", \"State\": \"Delhi\", \"Mobile Number\": \"xxxxxxx447\", \"Age Band\": \"20-30\"}",
				"ocr": {
					"id_number": "319644293458",
					"date_of_birth": "1991-08-24",
					"gender": "MALE",
					"state": "Uttarakhand",
					"phone_number": "098"
				},
				"government_output": {
					"aadhaar_number": "319644293458",
					"Gender": "MALE",
					"State": "Uttarakhand",
					"phone_number": "650",
					"age_band": "20-30"
				},
				"matched_information": {
					"message": "OCR Data has been verified with government source",
					"gender_match": true,
					"state_match": true,
					"age_match": true,
					"id_match": true,
					"partial_phone_number_match": false
				}
			 } 

**gender_match** will be true if gender from ocr and government are same.

**state_match** will be true if state from ocr and government are same.

**age_match** will be true if age from ocr and government are same.

**id_match** will be true if aadhaarId from ocr is same as government retrieved aadhaarId.

**partial_phone_number_match** will be true if last three digits of scanned phone Number is same as last three digits of government retrieved phone Number.

GST Certficate:
****************

**success Response**

**OCR**

.. code-block:: json
	  
					{
						"got_ocr_response": true,
						"got_gov_response": true,
						"result": "id_found",
						"message": "Id was found in the source",
						"success": true,
						"ocr": {
							"address": "FIRST AND FOURTH FLOOR, NO 20, LAKSHMI PLAZA, KRISHNANAGAR INDUSTRIAL LAYOUT, HOSUR ROAD, BANGALORE, Bengaluru (Bangalore) Urban, Kamataka, 560029",
							"constitution_of_business": "Private Limited Company",
							"date_of_liability": "2017-07-24",
							"gstin": "29AAYCS8889G1ZZ",
							"is_provisional": false,
							"legal_name": "SPRINGROLE INDIA PRIVATE LIMITED",
							"pan_number": "AAYCS8889G",
							"trade_name": "",
							"type_of_registration": "Regular",
							"valid_upto": "2017-07-24"
						},
						"government_output": {
							"additional_place_of_business_fields": {
								"additional_place_of_business_address ": {
									"building_name": "LAKSHMI PLAZA, KRISHNANAGAR INDUSTRIAL LAYOUT",
									"city": "",
									"door_number": "No 20",
									"dst": "Bengaluru (Bangalore) Urban",
									"floor_number": "FOURTH FLOOR",
									"latitude": "",
									"location": "BANGALORE",
									"longitude": "",
									"pincode": "560029",
									"state_name": "Karnataka",
									"street": "HOSUR ROAD"
								},
								"nature_of_additional_place_of_business": "Supplier of Services, Export, Recipient of Goods or Services"
							},
							"centre_jurisdiction": "RANGE-ESD4",
							"centre_jurisdiction_code": "YV0405",
							"constitution_of_business": "Private Limited Company",
							"date_of_cancellation": null,
							"date_of_registration": "2017-07-24",
							"gstin": "29AAYCS8889G1ZZ",
							"gstin_status": "Active",
							"last_updated_date": "2020-12-08",
							"legal_name": "SPRINGROLE INDIA PRIVATE LIMITED",
							"nature_of_business_activity": [
								"Export",
								"Supplier of Services",
								"Recipient of Goods or Services"
							],
							"principal_place_of_business_fields": {
								"nature_of_principal_place_of_business": "Export, Supplier of Services, Recipient of Goods or Services",
								"principal_place_of_business_address": {
									"building_name": "AMAR PLAZA, KRISHNANAGAR INDUSTRIAL LAYOUT",
									"city": "",
									"door_number": "NO 19",
									"dst": "Bengaluru (Bangalore) Urban",
									"floor_number": "SECOND FLOOR",
									"latitude": "",
									"location": "BANGALORE",
									"longitude": "",
									"pincode": "560029",
									"state_name": "Karnataka",
									"street": "HOSUR ROAD"
								}
							},
							"source": null,
							"state_jurisdiction_code": "KA011",
							"status": "id_found",
							"taxpayer_type": "Regular",
							"trade_name": "SPRINGROLE INDIA PRIVATE LIMITED"
						},
						"matched_information": {
							"message": "OCR Data has been verified with government source",
							"status": "id_found",
							"gstin_match": true,
							"legal_name_match": 100,
							"address_match": 79.70479704797047,
							"type_of_registration_match": true,
							"constitution_of_business_match": true,
							"date_of_liability_match": true
						}
					}

**gstin_match** will be true if gstin from ocr and goverment are same.

**legal_name_match** will be percentage match  of scanned legal_name and government retrieved legal_name.

**address_match** will be percentage match of scanned address and government retreived address.

**type_of_registration_match** will be true if type_of_registration from ocr and government are same

**constitution_of_business_match** will be true if constitution_of_business from ocr and government are same

**date_of_liability_match** will be true if date_of_liability from ocr and government are same

**NO OCR**

.. code-block:: json
	  
					{
						"got_gov_response": true,
						"result": "id_found",
						"message": "Id was found in the source",
						"success": true,
						"ocr": {
							"gstin": "29AAYCS8889G1ZZ",
							"legal_name": "SPRINGROLE INDIA PRIVATE LIMITED",
						},
						"government_output": {
							"additional_place_of_business_fields": {
								"additional_place_of_business_address ": {
									"building_name": "LAKSHMI PLAZA, KRISHNANAGAR INDUSTRIAL LAYOUT",
									"city": "",
									"door_number": "No 20",
									"dst": "Bengaluru (Bangalore) Urban",
									"floor_number": "FOURTH FLOOR",
									"latitude": "",
									"location": "BANGALORE",
									"longitude": "",
									"pincode": "560029",
									"state_name": "Karnataka",
									"street": "HOSUR ROAD"
								},
								"nature_of_additional_place_of_business": "Supplier of Services, Export, Recipient of Goods or Services"
							},
							"centre_jurisdiction": "RANGE-ESD4",
							"centre_jurisdiction_code": "YV0405",
							"constitution_of_business": "Private Limited Company",
							"date_of_cancellation": null,
							"date_of_registration": "2017-07-24",
							"gstin": "29AAYCS8889G1ZZ",
							"gstin_status": "Active",
							"last_updated_date": "2020-12-08",
							"legal_name": "SPRINGROLE INDIA PRIVATE LIMITED",
							"nature_of_business_activity": [
								"Export",
								"Supplier of Services",
								"Recipient of Goods or Services"
							],
							"principal_place_of_business_fields": {
								"nature_of_principal_place_of_business": "Export, Supplier of Services, Recipient of Goods or Services",
								"principal_place_of_business_address": {
									"building_name": "AMAR PLAZA, KRISHNANAGAR INDUSTRIAL LAYOUT",
									"city": "",
									"door_number": "NO 19",
									"dst": "Bengaluru (Bangalore) Urban",
									"floor_number": "SECOND FLOOR",
									"latitude": "",
									"location": "BANGALORE",
									"longitude": "",
									"pincode": "560029",
									"state_name": "Karnataka",
									"street": "HOSUR ROAD"
								}
							},
							"source": null,
							"state_jurisdiction_code": "KA011",
							"status": "id_found",
							"taxpayer_type": "Regular",
							"trade_name": "SPRINGROLE INDIA PRIVATE LIMITED"
						},
						"matched_information": {
							"message": "OCR Data has been verified with government source",
							"status": "id_found",
							"gstin_match": true,
							"legal_name_match": 100
						}
					}

**gstin_match** will be true if gstin from ocr and goverment are same.

**legal_name_match** will be percentage match  of scanned legal_name and government retrieved legal_name.

Passport
********

**success Response**

**OCR**

.. code-block:: json

			{
				"got_ocr_response": true,
				"got_MRZ_response": true,
				"result": "id_found",
				"message": "PASSPORT is Active and the details are matching with MRZ.",
				"error": "",
				"success": true,
				"ocr": {
					"address": "387 BANSDRONI PARK KOLKATA, KOLKATA",
					"date_of_birth": "1992-03-20",
					"date_of_expiry": "2024-08-26",
					"date_of_issue": "2014-08-27",
					"district": "KOLKATA",
					"fathers_name": "GHOSAL",
					"first_name": "MADHUMITA",
					"gender": "FEMALE",
					"id_number": "M1516926",
					"is_scanned": "false",
					"last_name": "GHOSAL",
					"mothers_name": "PURNIMA GHOSAL",
					"name_of_spouse": null,
					"name_on_card": "MADHUMITA GHOSAL",
					"nationality": null,
					"pincode": "700070",
					"place_of_birth": "TARKESHWAR, WEST BENGAL",
					"place_of_issue": "KOLKATA OSALE ABANDE",
					"state": "West Bengal"
				},
				"government_output": {
					"id_number": "M1516926",
					"first_name": "MADHUMITA",
					"last_name": "GHOSAL",
					"name_on_card": "MADHUMITA GHOSAL",
					"gender": "F",
					"MRZ_Verified": true
				},
				"matched_information": {
					"message": "OCR Data has been verified with MRZ",
					"first_name_match": 100,
					"last_name_match": 100,
					"ocr_id_match": true
				} 
			}

**ocr_id_match** will be true if passport_id from ocr and MRZ are same.

**first_name_match** will be percentage match  of scanned first_name and MRZ retreived first_name.

**last_name_match** will be percentage match  of scanned last_name and MRZ retreived last_name.


Bank Account Validation:
************************

**Success Response**

.. code-block:: json
	  
			 {
   				"got_gov_response": true,
   				"result": "id_found",
   				"information": "{\"name\":\"JOHN DOE\",\"account_number\":\"026291800001191\",\"ifsc\":\"YESB0000262\",\"accountExists\":\"YES\"}",
   				"message": "Bank Account details verified successfully.",
   				"success": true,
   				"ocr": {
       				   "name": "John Doe",
       				   "phone": "9393877270",
       				   "bankAccount": "026291800001191",
       				   "ifsc": "YESB0000262"
   				},
   				"government_output": {
       				    "name": "JOHN DOE",
       				    "account_number": "026291800001191",
       				    "ifsc": "YESB0000262",
       				    "accountExists": "YES"
   				},
   				"matched_information": {
       				    "name_match": 100,
       				    "account_number_match": true,
       				    "ifsc_match": true
   				}
			 }

**name_match** will be percentage match of name in OCR and government retreived name.

**account_number_match** will be true if account_number in OCR is same as government retreived account_number.

**ifsc_match** will be true if ifsc in OCR is same as government retreived ifsc.

UPI ID Validation:
************************

**Success Response**

.. code-block:: json
	  
		  {
   			"got_gov_response": true,
   			"result": "id_found",
   			"information": "{\"name\":\"John Doe\",\"vpa\":\"success@upi\",\"accountExists\":\"YES\"}",
   			"message": "VPA verification successful",
   			"success": true,
   			"ocr": {
       			    "name": "John Doe",
       			    "vpa": "success@upi"
   			},
   			"government_output": {
       			    "name": "John Doe",
       			    "vpa": "success@upi",
       			    "accountExists": "YES"
   			},
   			"matched_information": {
       			    "name_match": 100,
       			    "vpa_match": true
   			}
		  }  

**name_match** will be percentage match of name in OCR and government retreived name.

**vpa_match** will be true if vpa in OCR is same as government retreived vpa.

.. _appendex2:

Appendex 2
----------

**success response**

.. code-block:: json
		
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
					"docType": "ind_aadhaar",
					"document1": "https://pdf-reports-springrole.s3.amazonaws.com/adhaar.png",
					"belongsTo": "5df9fdf971b57d2c188ebc62",
					"got_face_match": true,
					"got_ocr_response": true,
					"got_gov_response": true,
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

.. code-block:: json
		
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
				}
				],
				"status": "completed",
				"query": {
					"name": "Piyush",
					"address": "897h9h7977997",
					"fatherName": "Sanjay "
				},
				"createdAt": "2020-03-16T14:07:46.285Z",
				"updatedAt": "2020-03-16T14:07:46.285Z",
				"__v": 0
	            }
	
**year** denotes the year in which the court case is registered.

**state_name** denotes the state in which the court case has been registered.

**case_category** denotes the category of the court case

**uniq_case_id** Unique id assigned to the court case
