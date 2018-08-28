swagger: "2.0"
x-collection-name: Aspose
x-complete: 1
info:
  title: Aspose
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: api.aspose.com
basePath: /v1.1
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