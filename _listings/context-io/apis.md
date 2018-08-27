---
name: Context.IO
x-slug: context-io
description: Create simple email webhooks and code against a free, RESTful, IMAP API.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
x-kinRank: "9"
x-alexaRank: "569975"
tags: "311"
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/context-io/apis.md
specificationVersion: "0.14"
apis:
- name: Context.IO - Get Accounts Threads Thread
  x-api-slug: accountsidthreadsthread-id-get
  description: |-
    Returns files, contacts and messages on a given thread. The purpose is to allow Gmail extensions to easily retrieve data when users's load a conversation in the Gmail UI. Hence, threads are identified by the value of their Gmail thread prefixed with "gm-".
    For example, if the URL of a conversation in the Gmail UI is https://mail.google.com/mail/u/0/#mbox/13119ab37f00b826, you would obtain the details about this thread by calling:
    GET https://api.context.io/2.0/accounts/<accountId>/threads/gm-13119ab37f00b826

    What about threads on non-Gmail mailboxes?
    You can retrieve thread information for any message using the Thread resource of that message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/172-context-io.jpg
  humanURL: http://context.io/
  baseURL: https://api.context.io//2.0/
  tags: API LIfeyclessss, Stack Network, Technology, SaaS, Mobile, API Provider, Emails,
    Messages, Profiles, Emails, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/context-io/accountsidthreadsthread-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/311/master/_listings/context-io/accountsidthreadsthread-id-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://constant.contact.api.gallery.streamdata.io
- type: x-api-stack
  url: http://context.io.stack.network
- type: x-base
  url: https://api.context.io/
- type: x-blog
  url: http://blog.context.io/
- type: x-blog-rss
  url: http://blog.context.io/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/product/context-io
- type: x-crunchbase
  url: https://crunchbase.com/organization/context-io
- type: x-documentation
  url: http://context.io/docs/2.0
- type: x-email
  url: hello@context.io
- type: x-email
  url: support@context.io
- type: x-email
  url: business@context.io
- type: x-faq
  url: http://context.io/privacy-faq
- type: x-github
  url: https://github.com/contextio
- type: x-ios-library
  url: https://github.com/contextio/contextio-ios
- type: x-node-js-library
  url: https://github.com/contextio/ContextIO-node
- type: x-php-library
  url: https://github.com/contextio/PHP-ContextIO
- type: x-pricing
  url: http://context.io/pricing
- type: x-privacy
  url: http://www.returnpath.com/privacy-policy-data
- type: x-python-library
  url: https://github.com/contextio/Python-ContextIO
- type: x-ruby-library
  url: https://github.com/contextio/contextio-ruby
- type: x-selfservice-registration
  url: http://context.io/#signup
- type: x-terms-of-service
  url: http://context.io/terms-of-service
- type: x-twitter
  url: https://twitter.com/contextio
- type: x-website
  url: http://context.io/
- type: x-website
  url: http://context.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---