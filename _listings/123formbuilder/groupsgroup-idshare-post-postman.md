{
  "info": {
    "name": "123FormBuilder Share a group with a user",
    "_postman_id": "b3139355-bf97-44af-96ab-4d02a61f14ec",
    "description": "This may not be available for your account. It is specific to certain users.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ping",
      "item": [
        {
          "id": "d37d4ed5-7991-458c-a86c-db04ced32cfb",
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
              "id": "c449d01f-139b-4106-a302-3e355c48fe46"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "bc211a93-39dd-4390-8ca8-bb5d6e4740dd",
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
              "id": "70aff34e-bb2a-40a8-b27a-2f8831f949f9"
            }
          ]
        },
        {
          "id": "8948008b-687f-4894-8f3f-910822ee9d27",
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
              "id": "fd2979cc-5180-4899-92cf-f5d3b7f701b8"
            }
          ]
        }
      ]
    },
    {
      "name": "Refresh",
      "item": [
        {
          "id": "9aa198dd-4f05-4f9b-8cbb-e148b55babe9",
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
              "id": "6201d93a-baf0-470c-b50a-08f4f7bebb08"
            }
          ]
        }
      ]
    },
    {
      "name": "Invalidate",
      "item": [
        {
          "id": "b23c5407-b463-457c-901b-7c04c6d94053",
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
              "id": "c2a317e8-7f7d-4c04-a065-6848cd817c7b"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "6eb5c86f-8683-44d5-9606-c77b8fd8c6a6",
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
              "id": "3e1ba588-960f-42e5-841e-cf40612d6762"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "2ae6cbbe-0373-4726-8e1e-ba32fa00104c",
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
              "id": "ce285d5a-8860-440a-bde4-063160e14932"
            }
          ]
        },
        {
          "id": "de588630-c493-4095-9626-aa7d35fb1927",
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
              "id": "fa73c970-0a23-4689-b6d2-599ecd1fd3df"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "1da1b175-fe55-4a9d-8065-73fd5db9d894",
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
              "id": "f25175be-2984-4b70-b871-98d4181e9bd1"
            }
          ]
        }
      ]
    },
    {
      "name": "Form",
      "item": [
        {
          "id": "35c753cf-069f-41cc-9a55-340f846397ae",
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
              "id": "8d3523c8-389e-464b-a9b3-9050e14c044d"
            }
          ]
        },
        {
          "id": "1763261b-1b39-4b6d-a7ab-a8a0c040c5b7",
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
              "id": "4a8922ad-4d85-443c-8d20-95c8e75f740e"
            }
          ]
        },
        {
          "id": "c3bbdf5b-3b8c-4f0c-abd6-375dbea87318",
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
              "id": "a475fa99-4fae-491a-8e37-f2400fc76e43"
            }
          ]
        },
        {
          "id": "d9a13478-72cc-4501-9b6e-4482cdfc9158",
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
              "id": "c24e3a2f-08e5-48cc-8129-1ed6ea7c7321"
            }
          ]
        },
        {
          "id": "e6f25572-d48e-438b-89a7-7014f892d7c5",
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
              "id": "69890c43-d3d3-41e5-8825-94d17b0968c4"
            }
          ]
        }
      ]
    },
    {
      "name": "Submissions",
      "item": [
        {
          "id": "296f906c-d9b0-48fb-906b-118b42840baf",
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
              "id": "1dbabc3e-e94d-4340-bb9e-3ee6d16088dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Submission",
      "item": [
        {
          "id": "b5250bda-5a7c-4660-af42-39e89a034fe5",
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
              "id": "0aa3cc2e-893b-43b2-b387-1b0759fac65f"
            }
          ]
        },
        {
          "id": "273d75f8-78a0-452c-95c2-844d5b0e6e83",
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
              "id": "6be0e060-0696-4687-a23c-24bc84659eb0"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "75819d46-b879-4c45-9bf7-777bfafeb292",
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
              "id": "e712310e-2661-4535-8c91-3249aa55942a"
            }
          ]
        },
        {
          "id": "8e8ba9ac-42f8-4635-b149-c4be08421e95",
          "name": "updates-the-details-of-a-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id"
              ],
              "variable": [
                {
                  "id": "group_id",
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
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "This is required when the webhook_url or parent_id is missing"
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
                  "description": "This is required when the name or parent_id is missing"
                }
              ]
            },
            "description": "Updates the details of a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "216a55ad-996e-4711-b715-ee00ae7e7d52"
            }
          ]
        }
      ]
    },
    {
      "name": "Forms",
      "item": [
        {
          "id": "7b85b252-c5eb-407b-8c48-59cb390b8575",
          "name": "displays-a-list-of-all-of-the-forms-within-a-specific-group",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id/forms"
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
            "description": "Displays a list of all of the forms within a specific group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e472ed6-8ad2-473b-a02c-ce66144c14b5"
            }
          ]
        }
      ]
    },
    {
      "name": "Share",
      "item": [
        {
          "id": "b80d7663-5e94-4068-8a76-986093b4763a",
          "name": "this-may-not-be-available-for-your-account-it-is-specific-to-certain-users",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id/share"
              ],
              "variable": [
                {
                  "id": "group_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
                  "key": "subuser_email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The username with whom you want to share this group"
                },
                {
                  "key": "subuser_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the user with whom you want to share this group"
                }
              ]
            },
            "description": "This may not be available for your account. It is specific to certain users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3519c7a-046b-4ecc-9aa0-761f5cb7e21b"
            }
          ]
        }
      ]
    }
  ]
}