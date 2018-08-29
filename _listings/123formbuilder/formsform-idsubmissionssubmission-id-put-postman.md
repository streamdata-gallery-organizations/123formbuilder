{
  "info": {
    "name": "123FormBuilder Update Submission",
    "_postman_id": "73270106-d003-4172-8621-c4a29cb35fdc",
    "description": "Update Submission",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ping",
      "item": [
        {
          "id": "58f64ef6-1f79-4f3f-8453-b55c75dbdff9",
          "name": "this-indicates-if-our-servers-are-up-and-running",
          "request": {
            "url": "http://api.123contactform.com/v2/ping",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This indicates if our servers are up and running."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3fc60e4-3483-4431-93da-412e82b40781"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "04e4c2e9-8f70-41cd-af74-6da067236e51",
          "name": "allows-you-to-authenticate-users-required-parameters-username-or-email-password-or-passhash",
          "request": {
            "url": "http://api.123contactform.com/v2/token?email=%7B%7D&passhash=%7B%7D&password=%7B%7D&username=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Allows you to authenticate users. \n\nRequired parameters:\n- username OR email\n- password OR passhash"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6984b0c0-e846-4298-95db-99e39ed059df"
            }
          ]
        }
      ]
    },
    {
      "name": "Refresh",
      "item": [
        {
          "id": "9717e882-4d88-45fe-b123-b93986a02432",
          "name": "refresh-token",
          "request": {
            "url": "http://api.123contactform.com/v2/token/refresh",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                }
              ]
            },
            "description": "Refresh token"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5762aa2d-1390-4544-ad5f-13df31b63ca0"
            }
          ]
        }
      ]
    },
    {
      "name": "Invalidate",
      "item": [
        {
          "id": "bbf1cb89-0985-4cf9-8e87-15eea194829c",
          "name": "invalidate-token",
          "request": {
            "url": "http://api.123contactform.com/v2/token/invalidate",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                }
              ]
            },
            "description": "Invalidate token"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94b6e5da-4fb3-4a44-bdc4-646528ba2f6f"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "1d90728a-4d17-4ecb-a457-b679316b1d0e",
          "name": "the-forms-endpoint-returns-information-about-the-forms-the-response-includes-submissions-and-other-d",
          "request": {
            "url": "http://api.123contactform.com/v2/forms?JWT=%7B%7D&page=%7B%7D&per_page=%7B%7D&search=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The forms endpoint returns information about the forms. The response includes submissions and other details about each form."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f83d9399-4343-48b9-92a7-07657a6c4c05"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "53139cfc-368f-441d-aa87-e23b605a43b7",
          "name": "create-a-new-form",
          "request": {
            "url": "http://api.123contactform.com/v2/forms",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "Form activity status"
                },
                {
                  "key": "active_date_from",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 1, this field is required"
                },
                {
                  "key": "active_date_to",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 1, this field is required"
                },
                {
                  "key": "active_days",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 4, this field is required"
                },
                {
                  "key": "group_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the group in which you want to create the form"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the new form"
                }
              ]
            },
            "description": "Create a new form"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b64db83-02e8-4a00-adbe-7e8173685986"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "e6dd9b3e-7834-4193-acd9-8e9a8299ad90",
          "name": "delete-multiple-forms",
          "request": {
            "url": "http://api.123contactform.com/v2/forms/bulk",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "form_ids",
                  "value": "{}",
                  "disabled": false,
                  "description": "The IDs of the forms separated by comma"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                }
              ]
            },
            "description": "Delete multiple forms"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a449b3d-6e48-4e3f-9501-778fca0c4d12"
            }
          ]
        }
      ]
    },
    {
      "name": "Form",
      "item": [
        {
          "id": "094b19ec-921d-402e-9a9e-cbcd8bf47fb1",
          "name": "get-the-details-of-a-single-form",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of a single form"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e53f3e83-6670-4550-85b1-8fa3af9d9711"
            }
          ]
        },
        {
          "id": "377c2c05-371e-45de-8dbb-e1420ee9e87d",
          "name": "update-form-details",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "active",
                  "value": "{}",
                  "disabled": false,
                  "description": "Form activity status"
                },
                {
                  "key": "active_date_from",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 1, this field is required"
                },
                {
                  "key": "active_date_to",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 1, this field is required"
                },
                {
                  "key": "active_days",
                  "value": "{}",
                  "disabled": false,
                  "description": "If activity status is 4, this field is required"
                },
                {
                  "key": "group_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the group in which you want to create the form"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Change the name of the form"
                }
              ]
            },
            "description": "Update form details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5eec9582-aa3b-40ba-8068-a54442d9bb28"
            }
          ]
        },
        {
          "id": "d8e68497-574b-4bb9-88a2-56cc6d313db4",
          "name": "delete-a-form",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id"
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                }
              ]
            },
            "description": "Delete a form"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da1d49e1-22fc-4ba5-be4c-f3545fc7d74f"
            }
          ]
        },
        {
          "id": "824774b0-cc85-4393-9e40-11a9c26f4c89",
          "name": "get-the-details-of-a-single-form-and-its-fields",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/fields"
              ],
              "query": [
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of a single form and its fields"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2367cbe-bb18-4b55-b6dd-7b6aa27615ef"
            }
          ]
        }
      ]
    },
    {
      "name": "Submissions",
      "item": [
        {
          "id": "70669475-0489-4960-b966-edbe99680ea2",
          "name": "get-all-submissions-received-through-a-form",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/submissions"
              ],
              "query": [
                {
                  "key": "include_recipients",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "per_page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_submission_id",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all submissions received through a form"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6afaf56e-0829-4c17-88ec-9943768810d4"
            }
          ]
        }
      ]
    },
    {
      "name": "Submission",
      "item": [
        {
          "id": "d1658ad9-074e-4abf-9ca9-71f351a95a16",
          "name": "get-the-details-of-a-single-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/submissions/:submission_id"
              ],
              "query": [
                {
                  "key": "include_recipients",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "submission_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the details of a single submission"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f5c81ad-affd-437c-a1b1-e242ce07023c"
            }
          ]
        },
        {
          "id": "f8ce495e-28cc-4cb1-9a52-ddbc950198b2",
          "name": "update-submission",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "forms/:form_id/submissions/:submission_id"
              ],
              "query": [
                {
                  "key": "approved",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "JWT",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "payed",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "form_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "submission_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update Submission"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c68de509-2a29-4d41-a2fa-78c87404ef65"
            }
          ]
        }
      ]
    }
  ]
}