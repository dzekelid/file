---
swagger: "2.0"
x-collection-name: Aspose
x-complete: 0
info:
  title: Aspose.Storage API Put Storage File Path
  description: The resource represents customers file at server file storage.
  termsOfService: http://www.aspose.com/corporate/legal/terms-of-use.aspx
  version: v1.1
host: api.aspose.com
basePath: /v1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /storage/file/{path}:
    delete:
      summary: Delete Storage File Path
      description: The resource represents customers file at server file sto
      operationId: deleteStorageFilePath
      x-api-path-slug: storagefilepath-delete
      responses:
        200:
          description: OK
      tags:
      - Storage
      - File
      - Path
    get:
      summary: Get Storage File Path
      description: The resource represents customers file at server file storage.
      operationId: getStorageFilePath
      x-api-path-slug: storagefilepath-get
      responses:
        200:
          description: OK
      tags:
      - Storage
      - File
      - Path
    post:
      summary: Post Storage File Path
      description: The resource represents customers file at server file storage
      operationId: postStorageFilePath
      x-api-path-slug: storagefilepath-post
      responses:
        200:
          description: OK
      tags:
      - Storage
      - File
      - Path
    put:
      summary: Put Storage File Path
      description: The resource represents customers file at server file storage.
      operationId: putStorageFilePath
      x-api-path-slug: storagefilepath-put
      responses:
        200:
          description: OK
      tags:
      - Storage
      - File
      - Path
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