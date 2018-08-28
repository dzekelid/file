swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/files/{fileID}:
    get:
      summary: Get a file
      description: Get a file.
      operationId: V2FilesByFileIDGet
      x-api-path-slug: v2filesfileid-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: fileID
      responses:
        200:
          description: Successful response
      tags:
      - File
    delete:
      summary: Delete a file
      description: Delete a file.
      operationId: V2FilesByFileIDDelete
      x-api-path-slug: v2filesfileid-delete
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: fileID
      responses:
        200:
          description: Successful response
      tags:
      - File
  /v2/files:
    post:
      summary: Create a file
      description: Create a file.
      operationId: V2FilesPost
      x-api-path-slug: v2files-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - File