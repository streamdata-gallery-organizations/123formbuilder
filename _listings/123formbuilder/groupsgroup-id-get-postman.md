{
  "info": {
    "name": "123FormBuilder Get group details",
    "_postman_id": "1549aada-9e8e-4b86-bde6-d196030ff7d8",
    "description": "Get information about a specific group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ping",
      "item": [
        {
          "id": "ca7c1c16-055d-4cf9-9e17-3b954c4e1b72",
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
              "id": "ebf02ca7-31cd-42f9-ab8e-dd657450fb33"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "82098434-f639-462b-a1d3-d6f04d9f1a35",
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
              "id": "e4837f70-335b-408a-a0ea-7b009c1043a6"
            }
          ]
        },
        {
          "id": "8034bb6a-560a-437c-9130-3d8c3a46416a",
          "name": "get-all-user-groups",
          "request": {
            "url": "http://api.123contactform.com/v2/groups?JWT=%7B%7D&page=%7B%7D&per_page=%7B%7D",
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
            "description": "Get all user groups"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f66ee5ce-f401-4a0d-9ef0-b951812544da"
            }
          ]
        }
      ]
    },
    {
      "name": "Refresh",
      "item": [
        {
          "id": "38a92b7c-8dd5-4c79-b2a0-eb44ba8f63da",
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
              "id": "a103ce67-e4d8-45e1-b763-4cf2db388937"
            }
          ]
        }
      ]
    },
    {
      "name": "Invalidate",
      "item": [
        {
          "id": "af6a8179-e354-4398-b40a-02b80f449f54",
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
              "id": "2b01418b-ff2f-4d08-9210-9b12df2132df"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "865ad422-a526-4d98-8644-143535fa26e2",
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
              "id": "3c840f7e-d12e-422a-a3f9-b389fe7243a3"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "1d87a88e-8a58-4285-8783-2d58c04899dd",
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
              "id": "4b88de07-71d6-4617-b371-ac3e48b376fe"
            }
          ]
        },
        {
          "id": "6773aabd-2b13-4058-92a2-892b8a3be16d",
          "name": "create-a-new-group",
          "request": {
            "url": "http://api.123contactform.com/v2/groups",
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
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Form name"
                },
                {
                  "key": "parent_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "Indicates the ID of the parent group"
                },
                {
                  "key": "webhook_url",
                  "value": "{}",
                  "disabled": false,
                  "description": "The URL of the WebHook"
                }
              ]
            },
            "description": "Create a new group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "667059f3-5e36-4ddd-9cb1-e83fc6818933"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "28e9d79b-7ef2-4591-afc4-412ec5850037",
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
              "id": "ec37f93b-3e96-4674-af84-455a8eddfc91"
            }
          ]
        }
      ]
    },
    {
      "name": "Form",
      "item": [
        {
          "id": "79605613-4183-46f1-8e52-2471e2829b64",
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
              "id": "3c30ecf3-4fdf-456e-919b-99cf995008d7"
            }
          ]
        },
        {
          "id": "99ff0239-16bc-4274-8d4b-9053f963c79a",
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
              "id": "75a9e875-0944-48ed-9001-64c66a341c7f"
            }
          ]
        },
        {
          "id": "cdacd8d6-aeee-4778-8f6c-20da54391167",
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
              "id": "80e9cb37-0d83-4805-b5e9-e4fc1cb9c2d5"
            }
          ]
        },
        {
          "id": "9d441932-6610-402f-8a13-f6bd1b393e33",
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
              "id": "1878bb81-99ac-40b8-b321-23e0382d7791"
            }
          ]
        },
        {
          "id": "51489748-03c2-42ea-9aac-744a1b6370b3",
          "name": "delete-one-form-submission",
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
            "method": "DELETE",
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
            "description": "Delete one form submission"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "169a9f4f-05c6-45c6-834f-a6512826874a"
            }
          ]
        }
      ]
    },
    {
      "name": "Submissions",
      "item": [
        {
          "id": "feab7e8b-9a7c-47d5-a316-5ba647256a65",
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
              "id": "c35087c2-29f6-4926-94c7-890ad83c3388"
            }
          ]
        }
      ]
    },
    {
      "name": "Submission",
      "item": [
        {
          "id": "229bc488-bbdc-45aa-b458-5f3c5e2c33bd",
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
              "id": "ca729171-0115-4d9b-8d3a-67796817a820"
            }
          ]
        },
        {
          "id": "016d56fd-5233-4aa0-89f6-20e7747576ce",
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
              "id": "b370f198-02bc-44ef-95d4-5aa8e05c9dd3"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "d7affa3d-e21e-4dba-9909-c96f3877e6f0",
          "name": "get-information-about-a-specific-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id"
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
                  "id": "group_id",
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
            "description": "Get information about a specific group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9e15b5e-ba4f-4311-9f06-bbbb90f3d0fb"
            }
          ]
        }
      ]
    }
  ]
}