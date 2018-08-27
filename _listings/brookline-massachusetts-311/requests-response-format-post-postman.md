{
  "info": {
    "name": "Brookline Massachusetts 311 Create Service Request",
    "_postman_id": "eceb6552-c9b4-462d-8dc4-2c23b82c9925",
    "description": "Submit a new request for with specific details of a single service. Must provide a location via lat/long or address_string or address_id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "311",
      "item": [
        {
          "id": "a8286f46-4c0c-4f2e-98c8-0de3b6b487f4",
          "name": "get-the-service-request-id-from-a-temporary-token-this-is-unnecessary-if-the-response-from-creating-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "spot.brooklinema.gov",
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
              "id": "d0212b5c-e6f0-49ad-80cc-c4525552aa7a"
            }
          ]
        },
        {
          "id": "d9122f41-7fcf-4909-9624-232bc8cfd28e",
          "name": "define-attributes-associated-with-a-service-code-these-attributes-can-be-unique-to-the-cityjurisdict",
          "request": {
            "url": {
              "protocol": "http",
              "host": "spot.brooklinema.gov",
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
              "id": "5ebd73a7-0fe5-4f7b-8c59-5314df1d6179"
            }
          ]
        },
        {
          "id": "5764be95-d729-43ed-93cf-c3b354c3c62d",
          "name": "list-acceptable-service-request-types-and-their-associated-service-codes-these-request-types-can-be-",
          "request": {
            "url": {
              "protocol": "http",
              "host": "spot.brooklinema.gov",
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
              "id": "b090c2e5-f6a2-41cb-bccf-c3873396baea"
            }
          ]
        },
        {
          "id": "fff3372b-9bfa-4fbb-9db2-e41ea65dee7c",
          "name": "query-the-current-status-of-an-individual-request",
          "request": {
            "url": {
              "protocol": "http",
              "host": "spot.brooklinema.gov",
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
              "id": "5a39f1e5-f65c-45c5-a419-a0e46fa8ba16"
            }
          ]
        },
        {
          "id": "8b52935b-2c16-4c1d-b890-7ad5db725e89",
          "name": "submit-a-new-request-for-with-specific-details-of-a-single-service-must-provide-a-location-via-latlo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "spot.brooklinema.gov",
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
              "id": "02cd1de0-cf51-4abd-94dd-a629d1d30b12"
            }
          ]
        }
      ]
    }
  ]
}