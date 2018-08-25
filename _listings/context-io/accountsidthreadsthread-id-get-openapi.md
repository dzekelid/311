---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Threads Thread
  description: |-
    Returns files, contacts and messages on a given thread. The purpose is to allow Gmail extensions to easily retrieve data when users's load a conversation in the Gmail UI. Hence, threads are identified by the value of their Gmail thread prefixed with "gm-".
    For example, if the URL of a conversation in the Gmail UI is https://mail.google.com/mail/u/0/#mbox/13119ab37f00b826, you would obtain the details about this thread by calling:
    GET https://api.context.io/2.0/accounts/<accountId>/threads/gm-13119ab37f00b826

    What about threads on non-Gmail mailboxes?
    You can retrieve thread information for any message using the Thread resource of that message.
  version: 1.0.0
host: api.context.io
basePath: /2.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/threads/{thread_id}:
    get:
      summary: Get Accounts Threads Thread
      description: |-
        Returns files, contacts and messages on a given thread. The purpose is to allow Gmail extensions to easily retrieve data when users's load a conversation in the Gmail UI. Hence, threads are identified by the value of their Gmail thread prefixed with "gm-".
        For example, if the URL of a conversation in the Gmail UI is https://mail.google.com/mail/u/0/#mbox/13119ab37f00b826, you would obtain the details about this thread by calling:
        GET https://api.context.io/2.0/accounts/<accountId>/threads/gm-13119ab37f00b826

        What about threads on non-Gmail mailboxes?
        You can retrieve thread information for any message using the Thread resource of that message.
      operationId: getAccountThread_
      x-api-path-slug: accountsidthreadsthread-id-get
      parameters:
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: path
        name: thread_id
        description: A gmail_thread_id prefixed with gm-
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Threads
      - Thread
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