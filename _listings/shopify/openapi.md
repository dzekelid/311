---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
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
---