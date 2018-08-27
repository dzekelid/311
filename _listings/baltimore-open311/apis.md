---
name: Baltimore Open311
x-slug: baltimore-open311
description: Baltimore 311 helps residents make their neighborhoods more beautiful
  by reporting local issues including potholes, graffiti, and streetlight outages.
  Residents can track the status of reports they or other members of the community
  have submitted
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: "311"
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/apis.md
specificationVersion: "0.14"
apis:
- name: Open311 GeoReport API - Id Of Service_request Via Token
  x-api-slug: tokenstoken-id-response-format-get
  description: Get the service_request_id from a temporary token. This is unnecessary
    if the response from creating a service request does not contain a token.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
  humanURL: http://wiki.open311.org/GeoReport_v2/Servers
  baseURL: https://311.baltimorecity.gov//open311/v2/
  tags: Government, Open311, 311, API Provider, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/tokenstoken-id-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/tokenstoken-id-response-format-get-openapi.md
- name: Open311 GeoReport API - (extended) Definition Of A Service Type
  x-api-slug: servicesservice-code-response-format-get
  description: Define attributes associated with a service code. These attributes
    can be unique to the city/jurisdiction.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
  humanURL: http://wiki.open311.org/GeoReport_v2/Servers
  baseURL: https://311.baltimorecity.gov//open311/v2/
  tags: Government, Open311, 311, API Provider, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/servicesservice-code-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/servicesservice-code-response-format-get-openapi.md
- name: Open311 GeoReport API - Service Types
  x-api-slug: services-response-format-get
  description: List acceptable service request types and their associated service
    codes. These request types can be unique to the city/jurisdiction.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
  humanURL: http://wiki.open311.org/GeoReport_v2/Servers
  baseURL: https://311.baltimorecity.gov//open311/v2/
  tags: Government, Open311, 311, API Provider, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/services-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/services-response-format-get-openapi.md
- name: Open311 GeoReport API - Current Status
  x-api-slug: requestservice-request-id-response-format-get
  description: Query the current status of an individual request
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
  humanURL: http://wiki.open311.org/GeoReport_v2/Servers
  baseURL: https://311.baltimorecity.gov//open311/v2/
  tags: Government, Open311, 311, API Provider, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/requestservice-request-id-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/requestservice-request-id-response-format-get-openapi.md
- name: Open311 GeoReport API - Create Service Request
  x-api-slug: requests-response-format-post
  description: Submit a new request for with specific details of a single service.
    Must provide a location via lat/long or address_string or address_id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
  humanURL: http://wiki.open311.org/GeoReport_v2/Servers
  baseURL: https://311.baltimorecity.gov//open311/v2/
  tags: Government, Open311, 311, API Provider, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/requests-response-format-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/requests-response-format-post-openapi.md
- name: Open311 GeoReport API - Requests
  x-api-slug: requests-response-format-get
  description: Query the current status of multiple requests.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/baltimore311-logo.png
  humanURL: http://wiki.open311.org/GeoReport_v2/Servers
  baseURL: https://311.baltimorecity.gov//open311/v2/
  tags: Government, Open311, 311, API Provider, Profiles
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/requests-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/baltimore-open311/requests-response-format-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://aws.waf.api.gallery.streamdata.io
- type: x-website
  url: http://wiki.open311.org/GeoReport_v2/Servers
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---