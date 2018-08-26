---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/{requestId}/files:
    get:
      summary: Get Request Requestid Files
      description: Get request requestid files.
      operationId: getApiV1RequestRequestFiles
      x-api-path-slug: apiv1requestrequestidfiles-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Files
    post:
      summary: Post Request Requestid Files
      description: Post request requestid files.
      operationId: postApiV1RequestRequestFiles
      x-api-path-slug: apiv1requestrequestidfiles-post
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: file
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Files
  /api/v1/request/{requestId}/files/{fileId}:
    get:
      summary: Get Request Requestid Files Fileid
      description: Get request requestid files fileid.
      operationId: getApiV1RequestRequestFilesFile
      x-api-path-slug: apiv1requestrequestidfilesfileid-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: fileId
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Files
      - Fileid
    delete:
      summary: Delete Request Requestid Files Fileid
      description: Delete request requestid files fileid.
      operationId: deleteApiV1RequestRequestFilesFile
      x-api-path-slug: apiv1requestrequestidfilesfileid-delete
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: fileId
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Files
      - Fileid
---