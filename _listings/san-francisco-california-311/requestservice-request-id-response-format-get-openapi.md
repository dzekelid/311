---
swagger: "2.0"
x-collection-name: San Francisco California 311
x-complete: 0
info:
  title: San Francisco California 311 Current Status
  description: Query the current status of an individual request
  termsOfService: (depends on server instance for example NYC http://dev.cityofchicago.org/docs/api/tos)
  contact:
    name: Open311 community
    url: http://wiki.open311.org/GeoReport_v2/
    email: discuss@lists.open311.org
  version: 1.0.0
host: mobile311.sfgov.org
basePath: /open311/v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /tokens/{token_id}.{response_format}:
    get:
      summary: Id Of Service_request Via Token
      description: Get the service_request_id from a temporary token. This is unnecessary
        if the response from creating a service request does not contain a token.
      operationId: get-the-service-request-id-from-a-temporary-token-this-is-unnecessary-if-the-response-from-creating-
      x-api-path-slug: tokenstoken-id-response-format-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: token_id
      responses:
        200:
          description: OK
      tags:
      - "311"
      - Id
      - Service
      - Request
      - Via
      - Token
  /services/{service_code}.{response_format}:
    get:
      summary: (extended) Definition Of A Service Type
      description: Define attributes associated with a service code. These attributes
        can be unique to the city/jurisdiction.
      operationId: define-attributes-associated-with-a-service-code-these-attributes-can-be-unique-to-the-cityjurisdict
      x-api-path-slug: servicesservice-code-response-format-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: service_code
      responses:
        200:
          description: OK
      tags:
      - "311"
      - (extended)
      - Definition
      - Service
      - Type
  /services.{response_format}:
    get:
      summary: Service Types
      description: List acceptable service request types and their associated service
        codes. These request types can be unique to the city/jurisdiction.
      operationId: list-acceptable-service-request-types-and-their-associated-service-codes-these-request-types-can-be-
      x-api-path-slug: services-response-format-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - "311"
      - Service
      - Types
  /request/{service_request_id}.{response_format}:
    get:
      summary: Current Status
      description: Query the current status of an individual request
      operationId: query-the-current-status-of-an-individual-request
      x-api-path-slug: requestservice-request-id-response-format-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: service_request_id
        description: Is specified in the main URL path rather than an added query
          string parameter
      responses:
        200:
          description: OK
      tags:
      - "311"
      - Current
      - Status
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---