{
  "info": {
    "name": "123FormBuilder Ping status",
    "_postman_id": "3450e923-5bc1-4b8b-8f01-2ca7f02c0a05",
    "description": "This indicates if our servers are up and running.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ping",
      "item": [
        {
          "id": "3c66e752-ae63-4655-9b22-359699d95b9a",
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
              "id": "21f26aea-0bf4-4b08-a9be-5a26cb934a04"
            }
          ]
        }
      ]
    }
  ]
}