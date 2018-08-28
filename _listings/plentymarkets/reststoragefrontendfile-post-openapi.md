---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Upload a single file to frontend storage.
  description: If file is an image, generate a thumbnail and store dimensions in metadata.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/storage/frontend/file:
    get:
      summary: Get file information for a single object in frontend storage. Append
        public cloudfront url to retrieved object.
      description: Get file information for a single object in frontend storage. append
        public cloudfront url to retrieved object..
      operationId: getRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-get
      parameters:
      - in: query
        name: key
        description: The key of the object to get information about
      responses:
        200:
          description: OK
      tags:
      - File
      - Informationa
      - Single
      - Object
      - In
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Retrieved
      - Object
    post:
      summary: Upload a single file to frontend storage.
      description: If file is an image, generate a thumbnail and store dimensions
        in metadata.
      operationId: postRestStorageFrontendFile
      x-api-path-slug: reststoragefrontendfile-post
      parameters:
      - in: query
        name: key
        description: The key for the uploaded object
      - in: query
        name: maxAge
        description: Number of seconds until the content of the file expires
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Single
      - File
      - To
      - Frontend
      - Storage
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