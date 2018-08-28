---
swagger: "2.0"
x-collection-name: Aspose
x-complete: 0
info:
  title: Aspose.Storage API Delete Storage File Path
  description: The resource represents customers file at server file sto
  termsOfService: http://www.aspose.com/corporate/legal/terms-of-use.aspx
  version: v1.1
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