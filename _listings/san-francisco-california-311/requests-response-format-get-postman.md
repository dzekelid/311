{
  "info": {
    "name": "San Francisco California 311 Requests",
    "_postman_id": "a85329c9-eb96-4214-bbf3-39ad4d04134f",
    "description": "Query the current status of multiple requests.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "311",
      "item": [
        {
          "id": "aa7bcc56-1721-4662-a4d2-5966f2d7c370",
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
              "id": "48524f54-6bae-4cf4-a10f-925e875a134e"
            }
          ]
        },
        {
          "id": "fd670eaa-fb43-4eb3-b6de-396d8a0d0e1c",
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
              "id": "4855effc-d629-4b9e-aca0-f2ccc6d52c83"
            }
          ]
        },
        {
          "id": "8380f51f-2fee-41bb-af43-a99b3500479c",
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
              "id": "7a3c6624-8e6f-44b7-aba9-6a42e8f4dbae"
            }
          ]
        },
        {
          "id": "cc761b8c-9f4d-4ff8-9918-8003e9632436",
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
              "id": "1af4ff0b-0f1b-494c-9bc8-1fc759ecf844"
            }
          ]
        },
        {
          "id": "750b4222-0517-411d-897c-c1e8d8755098",
          "name": "query-the-current-status-of-multiple-requests",
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
              "id": "3b66f7fc-8605-4083-a778-6d8983f6b91d"
            }
          ]
        },
        {
          "id": "7431c9b1-db35-4fa6-a914-58d2edc4c0fa",
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
              "id": "ce2914b9-d1b7-48ef-a89f-67043784be43"
            }
          ]
        }
      ]
    }
  ]
}