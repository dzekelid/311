---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Activate a one-time charge
  description: Activate a one-time charge.
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/application_charges/675931192/activate.json:
    post:
      summary: Activate a one-time charge
      description: Activate a one-time charge.
      operationId: postAdminApplicationCharges675931192Activate.json
      x-api-path-slug: adminapplication-charges675931192activate-json-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Activate
      - One-time
      - Charge
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