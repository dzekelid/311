swagger: "2.0"
x-collection-name: Context.IO
x-complete: 1
info:
  title: Context.IO
  description: context-io-is-the-missing-email-api-that-makes-it-easy-and-fast-to-integrate-your-users-email-data-in-your-application-
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