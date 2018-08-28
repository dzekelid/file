---
swagger: "2.0"
x-collection-name: Context.IO
x-complete: 0
info:
  title: Context.IO Get Accounts Files Fileid Revisions
  description: Lists other revisions of a given file. Returns a list of revisions
    attached to other emails in the mailbox for a given file. Two files are considered
    revisions of the same document if their file names are identical outside of revision
    indicators such as dates, author initials, version numbers and keywords like "final"
    or "draft".
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
  /accounts/{id}/contacts/{email}/files:
    get:
      summary: Get Accounts Contacts Email Files
      description: Lists files exchanged with a contact. Returns the latest attachments
        exchanged with one or more email addresses. By "exchanged with Mr. X" we mean
        any file attached to an email received from Mr. X, sent to Mr. X or sent by
        anyone to both Mr. X and the mailbox owner.
      operationId: listAccountContactFiles_
      x-api-path-slug: accountsidcontactsemailfiles-get
      parameters:
      - in: path
        name: email
        description: Email address of a contact
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Contacts
      - Email
      - Files
  /accounts/{id}/files:
    get:
      summary: Get Accounts Files
      description: 'Lists files found as email attachments. List filters: each of
        the email, to, from, cc and bcc parameters can be set to a comma-separated
        list of email addresses. These multiple addresses are treated as an OR combination.
        You can set more than one parameter when doing this call. Multiple parameters
        are treated as an AND combination.'
      operationId: listAccountFiles_
      x-api-path-slug: accountsidfiles-get
      parameters:
      - in: query
        name: bcc
        description: Email address of a contact BCCed on the messages
      - in: query
        name: cc
        description: Email address of a contact CCed on the messages
      - in: query
        name: date_after
        description: Only include files attached to messages sent after a given timestamp
      - in: query
        name: date_before
        description: Only include files attached to messages sent before a given timestamp
      - in: query
        name: email
        description: Email address of the contact for whom you want the latest files
          exchanged with
      - in: query
        name: file_name
        description: Search for files based on their name
      - in: query
        name: from
        description: Email address of a contact files have been received from
      - in: query
        name: group_by_revisions
        description: If set to 1, the list will do an intelligent grouping of files
          to reflect occurrences of the same document
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      - in: query
        name: indexed_after
        description: Only include files attached to messages indexed after a given
          timestamp
      - in: query
        name: indexed_before
        description: Only include files attached to messages indexed before a given
          timestamp
      - in: query
        name: limit
        description: The maximum number of results to return
      - in: query
        name: offset
        description: Start the list at this offset (zero-based)
      - in: query
        name: to
        description: Email address of a contact files have been sent to
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
  /accounts/{id}/files/{fileId}:
    get:
      summary: Get Accounts Files Fileid
      description: Gets information about a given file.
      operationId: getAccountFile_
      x-api-path-slug: accountsidfilesfileid-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
  /accounts/{id}/files/{fileId}/changes:
    get:
      summary: Get Accounts Files Fileid Changes
      description: Lists files that can be compared with a given file.
      operationId: listComparableAccountFiles_
      x-api-path-slug: accountsidfilesfileidchanges-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Changes
  /accounts/{id}/files/{fileId}/content:
    get:
      summary: Get Accounts Files Fileid Content
      description: 'Downloads a given file. Returns the content a given attachment.
        On-demand data retrieval: since we do not keep full copies of attachments
        on our servers, the file has to be retrieved from the IMAP server when this
        call is made. If the IMAP server is unreachable at the time the call is made,
        this call will return an error.'
      operationId: getAccountFileContent_
      x-api-path-slug: accountsidfilesfileidcontent-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Content
  /accounts/{id}/files/{fileId}/related:
    get:
      summary: Get Accounts Files Fileid Related
      description: Lists other files related to a given file. Returns a list of files
        that are related to the given file. Currently, relation between files is based
        on how similar their names are.
      operationId: listAccountFileRelatedFiles_
      x-api-path-slug: accountsidfilesfileidrelated-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Related
  /accounts/{id}/files/{fileId}/revisions:
    get:
      summary: Get Accounts Files Fileid Revisions
      description: Lists other revisions of a given file. Returns a list of revisions
        attached to other emails in the mailbox for a given file. Two files are considered
        revisions of the same document if their file names are identical outside of
        revision indicators such as dates, author initials, version numbers and keywords
        like "final" or "draft".
      operationId: listAccountFileRevisions_
      x-api-path-slug: accountsidfilesfileidrevisions-get
      parameters:
      - in: path
        name: fileId
        description: Unique id of a file
      - in: path
        name: id
        description: Unique id of an account accessible through your API key
      responses:
        200:
          description: OK
      tags:
      - Accounts
      - Files
      - FileId
      - Revisions
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