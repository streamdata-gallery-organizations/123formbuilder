{
  "info": {
    "name": "123FormBuilder Create new account",
    "_postman_id": "f7d2caf9-afef-40ae-a74e-1a9b53ecf72a",
    "description": "Creates a new account (standalone user). This is available only upon request.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ping",
      "item": [
        {
          "id": "50354630-7d6b-4c3e-92d9-1de3a5c2368a",
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
              "id": "f9db8227-699f-497d-ac59-9de79f675ebd"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "bdbfe1db-f313-4658-8d44-9628a3418cf6",
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
              "id": "71f2bb1e-e551-4e6e-a3e9-a764a6290117"
            }
          ]
        },
        {
          "id": "48032325-9934-44ac-aa82-125a5a3e2629",
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
              "id": "fe847379-de80-46f3-b95e-71b75b70a36c"
            }
          ]
        },
        {
          "id": "5c6c04cc-e6ba-4bc3-8e3b-5f54674f4ff1",
          "name": "update-user-information",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "users/:identifier"
              ],
              "variable": [
                {
                  "id": "identifier",
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
                  "key": "admin",
                  "value": "{}",
                  "disabled": false,
                  "description": "Indicates if the subuser is admin or not"
                },
                {
                  "key": "allow_create_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow or restrict subuser access to creating new forms"
                },
                {
                  "key": "allow_delete_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow subusers to delete forms"
                },
                {
                  "key": "allow_duplicate_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow subusers to duplicate forms"
                },
                {
                  "key": "can_manage_groups",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow admin subusers to manage groups"
                },
                {
                  "key": "can_manage_users",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow admin subusers to manage users"
                },
                {
                  "key": "company_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the company to which the subuser belongs"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "Email address of the account"
                },
                {
                  "key": "JWT",
                  "value": "{}",
                  "disabled": false,
                  "description": "JWT authentication token"
                },
                {
                  "key": "passhash",
                  "value": "{}",
                  "disabled": false,
                  "description": "MD5 password"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "Plain text password"
                }
              ]
            },
            "description": "Update user information"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69855a82-4ebf-4b12-9b13-25d35b44eadf"
            }
          ]
        }
      ]
    },
    {
      "name": "Refresh",
      "item": [
        {
          "id": "530b10da-4306-4997-b435-18c6bf5fbdd8",
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
              "id": "9f03fd50-3383-42e6-9fc3-846de6739222"
            }
          ]
        }
      ]
    },
    {
      "name": "Invalidate",
      "item": [
        {
          "id": "394e58c3-de4b-4574-a6a8-4bc9a7049cdc",
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
              "id": "821f4b40-54e5-41e0-9cba-ac78671a3954"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "af4f9918-6c1e-4337-a1a5-41888b0bac9b",
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
              "id": "d1cd34dc-bc0f-4caf-a043-2b123dfc295f"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "17b45fb3-02ea-4632-b6bb-14c9ce824ad3",
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
              "id": "0acd98d8-6baa-40ac-a85a-d5956d904b18"
            }
          ]
        },
        {
          "id": "28c54d98-ceeb-4b83-acbf-d028cd826d4d",
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
              "id": "47ebe7cf-da37-4311-b30f-478ab0ee55b1"
            }
          ]
        },
        {
          "id": "48fc86fb-3341-405d-8112-eb0beaa6bec8",
          "name": "create-a-new-subuser",
          "request": {
            "url": "http://api.123contactform.com/v2/users",
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
                  "key": "admin",
                  "value": "{}",
                  "disabled": false,
                  "description": "Indicates if the subuser is admin or not"
                },
                {
                  "key": "allow_create_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow or restrict subuser access to creating new forms"
                },
                {
                  "key": "allow_delete_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow subusers to delete forms"
                },
                {
                  "key": "allow_duplicate_form",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow subusers to duplicate forms"
                },
                {
                  "key": "can_manage_groups",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow admin subusers to manage groups"
                },
                {
                  "key": "can_manage_users",
                  "value": "{}",
                  "disabled": false,
                  "description": "Allow admin subusers to manage users"
                },
                {
                  "key": "company_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The name of the company to which the subuser belongs"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "Email address of the account"
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
                  "description": "Username of the account"
                },
                {
                  "key": "passhash",
                  "value": "{}",
                  "disabled": false,
                  "description": "MD5 password"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "Plain text password"
                }
              ]
            },
            "description": "Create a new subuser"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b1e1401f-3a40-4dc4-bcdc-f56d0351d140"
            }
          ]
        },
        {
          "id": "ad770c57-9050-43eb-9275-893ec0583520",
          "name": "creates-a-new-account-standalone-user-this-is-available-only-upon-request",
          "request": {
            "url": "http://api.123contactform.com/v2/accounts",
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
                  "key": "company_name",
                  "value": "{}",
                  "disabled": false,
                  "description": "The company name associated with the account"
                },
                {
                  "key": "email",
                  "value": "{}",
                  "disabled": false,
                  "description": "The email address associated with the account"
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
                  "description": "The username associated with the account"
                },
                {
                  "key": "password",
                  "value": "{}",
                  "disabled": false,
                  "description": "The password associated with the account"
                },
                {
                  "key": "password_repeat",
                  "value": "{}",
                  "disabled": false,
                  "description": "Password repeat"
                },
                {
                  "key": "plan",
                  "value": "{}",
                  "disabled": false,
                  "description": "The service plan of the account: 0 - Free (default value), 1 - Gold, 2 - Platinum, 3 - Diamond"
                }
              ]
            },
            "description": "Creates a new account (standalone user). This is available only upon request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "acbf37b8-b8fe-4108-8138-4dd18d07074b"
            }
          ]
        }
      ]
    },
    {
      "name": "Multiple",
      "item": [
        {
          "id": "2907fdbf-16f6-4cf4-9450-7940ae16d4be",
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
              "id": "bd80e248-8fd1-4444-83a5-45341cbc7f3e"
            }
          ]
        }
      ]
    },
    {
      "name": "Form",
      "item": [
        {
          "id": "c8336f1f-176d-4320-bc10-d354527f2ba1",
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
              "id": "0d286dc6-775d-4a86-9efa-65c6c6ed3cda"
            }
          ]
        },
        {
          "id": "5d37d0c9-cc25-4c72-ad49-a0d6f474e7cb",
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
              "id": "31093306-df3c-47ef-840d-85c373cd1953"
            }
          ]
        },
        {
          "id": "edf4112d-794d-495f-9ea8-84fd3311f92a",
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
              "id": "cd78a805-34f7-4085-85b0-2e332d9132ab"
            }
          ]
        },
        {
          "id": "9af394ef-a53e-411c-ad0e-831ca1a9637a",
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
              "id": "cc9ff0ab-595f-4b1f-ac04-9ccd405ca584"
            }
          ]
        },
        {
          "id": "8d185978-af05-4dac-9573-4d4987e7af04",
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
              "id": "d4105afc-a88e-462c-ad8b-498f87fcc7ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Submissions",
      "item": [
        {
          "id": "d44c77fa-ef10-4f95-9327-76da04f7b8cb",
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
              "id": "0db327ae-0d25-4902-97bc-e7558234f7e4"
            }
          ]
        }
      ]
    },
    {
      "name": "Submission",
      "item": [
        {
          "id": "948a0720-d90a-43dc-83b5-405a596d651e",
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
              "id": "a663e08c-8657-4564-bf48-b07d9f7b123c"
            }
          ]
        },
        {
          "id": "a7bc7236-c1e5-472c-b156-c33450008290",
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
              "id": "afa9b26b-89d4-4343-8127-190c3dff76f0"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "934f2812-c32e-4cfe-966b-58375aca255e",
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
              "id": "1e1b179d-dd99-42db-af80-d48b1863ae53"
            }
          ]
        },
        {
          "id": "7c1818e9-e88d-4a3f-8492-d84467b52af0",
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
              "id": "40c0872a-9ba9-4f73-b525-10241bff0c67"
            }
          ]
        }
      ]
    },
    {
      "name": "Forms",
      "item": [
        {
          "id": "b15e7086-3ece-4d0a-a0c5-e0af04e7a29e",
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
              "id": "e0ff313b-96a7-4a90-b3fa-d0058637ece7"
            }
          ]
        }
      ]
    },
    {
      "name": "Share",
      "item": [
        {
          "id": "c388cb8a-3d2d-4b27-ae41-6ec7adaf2588",
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
              "id": "96aa1f90-d7b6-46e6-aa61-57c71fcea949"
            }
          ]
        }
      ]
    },
    {
      "name": "Unshare",
      "item": [
        {
          "id": "9858c0a8-5ab6-48b9-a615-6a7b5275b5b0",
          "name": "this-may-not-be-available-for-your-account-it-is-specific-to-certain-users",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.123contactform.com",
              "path": [
                "v2",
                "groups/:group_id/unshare"
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
                  "description": "The username from whom you want to unshare the group"
                },
                {
                  "key": "subuser_id",
                  "value": "{}",
                  "disabled": false,
                  "description": "The ID of the subuser from whom you want to unshare the group"
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
              "id": "4b5afe22-f222-46f2-9ae7-03122135f3c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "1f4cffc9-59f2-43e8-829c-1b2581765fc8",
          "name": "get-info-about-master-user-and-subusers",
          "request": {
            "url": "http://api.123contactform.com/v2/users?JWT=%7B%7D&page=%7B%7D&per_page=%7B%7D",
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
            "description": "Get info about master user and subusers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13d12ca0-5a16-4643-a261-6a04ad01c403"
            }
          ]
        }
      ]
    }
  ]
}