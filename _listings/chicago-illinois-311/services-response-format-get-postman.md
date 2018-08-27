{
  "info": {
    "name": "Chicago Illinois 311 Service Types",
    "_postman_id": "e8fc9ace-4393-43c8-996e-072bb5a1c4a2",
    "description": "List acceptable service request types and their associated service codes. These request types can be unique to the city/jurisdiction.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "311",
      "item": [
        {
          "id": "6a6eb6f1-1886-48c5-b0fb-725764e07885",
          "name": "get-the-service-request-id-from-a-temporary-token-this-is-unnecessary-if-the-response-from-creating-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "311api.cityofchicago.org",
              "path": [
                "open311",
                "v2",
                "tokens/:token_id.:response_format"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "token_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "response_format",
                  "value": "response_format",
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
            "description": "Get the service_request_id from a temporary token. This is unnecessary if the response from creating a service request does not contain a token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b282687f-817b-4687-84a4-430effe9b77e"
            }
          ]
        },
        {
          "id": "982558a1-3dc8-42f9-ab89-e157b61377f2",
          "name": "define-attributes-associated-with-a-service-code-these-attributes-can-be-unique-to-the-cityjurisdict",
          "request": {
            "url": {
              "protocol": "http",
              "host": "311api.cityofchicago.org",
              "path": [
                "open311",
                "v2",
                "services/:service_code.:response_format"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "service_code",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "response_format",
                  "value": "response_format",
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
            "description": "Define attributes associated with a service code. These attributes can be unique to the city/jurisdiction."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "baee16ad-62d8-4407-b225-a7db7a4da210"
            }
          ]
        },
        {
          "id": "f645f3f9-c410-41bb-817c-0133ce9a7a5e",
          "name": "list-acceptable-service-request-types-and-their-associated-service-codes-these-request-types-can-be-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "311api.cityofchicago.org",
              "path": [
                "open311",
                "v2",
                "services.:response_format"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "response_format",
                  "value": "response_format",
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
            "description": "List acceptable service request types and their associated service codes. These request types can be unique to the city/jurisdiction."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c791097-3783-4fad-9e00-5638885fef20"
            }
          ]
        }
      ]
    }
  ]
}