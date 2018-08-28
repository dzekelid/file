---
swagger: "2.0"
x-collection-name: SugarSync
x-complete: 0
info:
  title: Sugar Sync  API Retrieving File Information
  description: To retrieve information about a file, an application submits an HTTP
    GET request to then          file resource that represents the file.
  version: "1"
host: api.sugarsync.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /file:
    get:
      summary: Retrieving File Data
      description: To retrieve file data, an application submits an HTTP GET request
        to then          file data resource that represents the data for the file.
      operationId: retrieving-file-data
      x-api-path-slug: file-get
      responses:
        200:
          description: OK
      tags:
      - File
    put:
      summary: Uploading File Data
      description: An application can upload data to a file by issuing an HTTP PUT
        request to thenfile data resource that represents the data for the file.n
      operationId: uploading-file-data
      x-api-path-slug: file-put
      responses:
        200:
          description: OK
      tags:
      - File
  /file/:
    delete:
      summary: Deleting a File
      description: An application can permanently delete a file by issuing an HTTP
        DELETE request to the URL of thenfile resource.nIts a good idea to precede
        DELETE requests like this with a caution note in your applications user interface.n
      operationId: deleting-a-file
      x-api-path-slug: file-delete
      responses:
        200:
          description: OK
      tags:
      - File
    get:
      summary: Retrieving File Information
      description: To retrieve information about a file, an application submits an
        HTTP GET request to then          file resource that represents the file.
      operationId: retrieving-file-information
      x-api-path-slug: file-get
      responses:
        200:
          description: OK
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