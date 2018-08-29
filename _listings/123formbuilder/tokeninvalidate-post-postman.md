{
  "info": {
    "name": "123FormBuilder Invalidate token",
    "_postman_id": "9540227d-482c-4600-83ae-bba0b9a0d497",
    "description": "Invalidate token",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ping",
      "item": [
        {
          "id": "6e99132f-e35c-478f-a3de-d05ae3417be7",
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
              "id": "621ca5e6-4199-4ccc-b3a1-c58dd695a335"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "9536088b-3f02-46b4-8902-017dabb788e9",
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
              "id": "39753e14-6491-4b95-84a4-2cff5c89176e"
            }
          ]
        }
      ]
    },
    {
      "name": "Refresh",
      "item": [
        {
          "id": "b479fe07-2df9-4458-ae8f-e49092e6bccc",
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
              "id": "ac15001d-8ea0-4813-a100-6c7668090b6b"
            }
          ]
        }
      ]
    },
    {
      "name": "Invalidate",
      "item": [
        {
          "id": "c3cf47a8-6e22-47e8-aa9b-1830a30e84ba",
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
              "id": "35aad253-daf7-49ef-ab57-01f9ba638832"
            }
          ]
        }
      ]
    }
  ]
}