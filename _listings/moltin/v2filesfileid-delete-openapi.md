---
swagger: "2.0"
x-collection-name: moltin
x-complete: 0
info:
  title: Moltin API Delete a file
  description: Delete a file.
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