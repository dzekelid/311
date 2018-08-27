{
  "info": {
    "name": "San Francisco California 311 Create Service Request",
    "_postman_id": "3abfc2a1-2d7c-456f-9e2f-d35b9eb5366e",
    "description": "Submit a new request for with specific details of a single service. Must provide a location via lat/long or address_string or address_id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "311",
      "item": [
        {
          "id": "45a9cd83-72bc-4430-9ca0-327eae31fb42",
          "name": "get-the-service-request-id-from-a-temporary-token-this-is-unnecessary-if-the-response-from-creating-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "mobile311.sfgov.org",
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
              "id": "7408872d-d113-4dec-8b4a-e0c0595afc24"
            }
          ]
        },
        {
          "id": "fb693128-1d41-46af-a999-9c9084baa261",
          "name": "define-attributes-associated-with-a-service-code-these-attributes-can-be-unique-to-the-cityjurisdict",
          "request": {
            "url": {
              "protocol": "http",
              "host": "mobile311.sfgov.org",
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
              "id": "4e300124-2b30-43cc-93e5-8603d4e195de"
            }
          ]
        },
        {
          "id": "7cf70288-8c72-475d-9b78-e7e07d1a6c46",
          "name": "list-acceptable-service-request-types-and-their-associated-service-codes-these-request-types-can-be-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "mobile311.sfgov.org",
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
              "id": "ec172a69-b550-4d66-b549-bb2253a6b4dd"
            }
          ]
        },
        {
          "id": "cdaa8d04-b96f-4fce-89bf-f1426fa73bd1",
          "name": "query-the-current-status-of-an-individual-request",
          "request": {
            "url": {
              "protocol": "http",
              "host": "mobile311.sfgov.org",
              "path": [
                "open311",
                "v2",
                "request/:service_request_id.:response_format"
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
                  "id": "service_request_id",
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
            "description": "Query the current status of an individual request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "431641f2-fa61-4060-90d3-527044d036c0"
            }
          ]
        },
        {
          "id": "fd3d2509-bc0d-43f3-b500-69be891b19bb",
          "name": "submit-a-new-request-for-with-specific-details-of-a-single-service-must-provide-a-location-via-latlo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "mobile311.sfgov.org",
              "path": [
                "open311",
                "v2",
                "requests.:response_format"
              ],
              "query": [
                {
                  "key": "address_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "address_string",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "attribute",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lat",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "long",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "service_code",
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
            "description": "Submit a new request for with specific details of a single service. Must provide a location via lat/long or address_string or address_id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b28f107-76c6-456f-a7f1-17d04bd1e24c"
            }
          ]
        }
      ]
    }
  ]
}