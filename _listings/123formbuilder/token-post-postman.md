{
  "info": {
    "name": "123FormBuilder User login",
    "_postman_id": "611cd6d4-b22d-4329-a171-7de32e18eb6b",
    "description": "Allows you to authenticate users. \n\nRequired parameters:\n- username OR email\n- password OR passhash",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ping",
      "item": [
        {
          "id": "deec2b1a-833d-4771-ad0a-a1a0e08d19d5",
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
              "id": "26487755-fc8e-42dd-a3a7-69d2395ec225"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "c4e927b9-5813-493a-8109-b113d667b7a4",
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
              "id": "7455a42f-bc7e-46b1-b093-e711ddc27532"
            }
          ]
        }
      ]
    }
  ]
}