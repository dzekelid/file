---
swagger: "2.0"
x-collection-name: Xero
x-complete: 0
info:
  title: Clarity Accounting Post Accounts Attachments Filename
  description: Post accounts account attachments filename.
  contact:
    name: Xero Developer Team
    url: https://developer.xero.com
  version: "2.0"
host: api.xero.com
basePath: /api.xro/2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountID}/Attachments/{FileName}:
    get:
      summary: Get Accounts Attachments Filename
      description: Get accounts account attachments filename.
      operationId: getAccountsAccountAttachmentsFilename
      x-api-path-slug: accountsaccountidattachmentsfilename-get
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: path
        name: FileName
        description: The filename of the attachment to be downloaded
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
      - FileName
    post:
      summary: Post Accounts Attachments Filename
      description: Post accounts account attachments filename.
      operationId: postAccountsAccountAttachmentsFilename
      x-api-path-slug: accountsaccountidattachmentsfilename-post
      parameters:
      - in: path
        name: AccountID
        description: The Xero generated unique identifier for an account
      - in: body
        name: Content
        description: The raw content of the file to be uploaded
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: FileName
        description: The filename of the attachment being uploaded
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - AccountID
      - Attachments
      - FileName
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