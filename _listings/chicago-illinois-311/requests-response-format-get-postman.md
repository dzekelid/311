{
  "info": {
    "name": "Chicago Illinois 311 Requests",
    "_postman_id": "a7a5010f-f8ca-4427-93b2-20dda24d1417",
    "description": "Query the current status of multiple requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "311",
      "item": [
        {
          "id": "274ea4bd-8b02-43dc-9648-47f5b180f2ca",
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
              "id": "b73198b2-e2fd-4a64-ab89-40b1f42dad26"
            }
          ]
        },
        {
          "id": "a6a005fc-4f4b-47ce-ae89-992a05f263bf",
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
              "id": "2e0627a4-7c5d-48c9-a21c-31de68919680"
            }
          ]
        },
        {
          "id": "0cb7710b-0275-41f1-9d42-59bb53971804",
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
              "id": "bf6756a7-2248-4955-8d43-beb67a45b163"
            }
          ]
        },
        {
          "id": "20ea644c-fc0b-4493-9a19-2b2e418f01ee",
          "name": "query-the-current-status-of-an-individual-request",
          "request": {
            "url": {
              "protocol": "http",
              "host": "311api.cityofchicago.org",
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
              "id": "a9d61d02-d58a-4240-be0b-6470b5a6e6ac"
            }
          ]
        },
        {
          "id": "403b4d47-6254-430a-ba7a-85c7c1c7e39f",
          "name": "query-the-current-status-of-multiple-requests",
          "request": {
            "url": {
              "protocol": "http",
              "host": "311api.cityofchicago.org",
              "path": [
                "open311",
                "v2",
                "requests.:response_format"
              ],
              "query": [
                {
                  "key": "end_date",
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
                },
                {
                  "key": "service_request_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "status",
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
            "description": "Query the current status of multiple requests."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1a22bbd-5b38-44f0-a1f1-be4adcda2e7f"
            }
          ]
        },
        {
          "id": "e55be110-dd0a-4586-81a1-e486314f044b",
          "name": "submit-a-new-request-for-with-specific-details-of-a-single-service-must-provide-a-location-via-latlo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "311api.cityofchicago.org",
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
              "id": "aa8b615f-638e-4615-889a-7b7dace43d46"
            }
          ]
        }
      ]
    }
  ]
}