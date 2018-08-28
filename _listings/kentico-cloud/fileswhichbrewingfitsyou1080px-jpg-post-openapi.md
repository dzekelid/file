---
swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 0
info:
  title: Kentico Cloud Upload a binary file
  description: "Add a new file. The uploaded file will not be visible in the Kentico
    Cloud UI unless there is an asset using it, see how to [add an asset](https://developer.kenticocloud.com/v1/reference#content-management-api-add-asset).\r\n\r\n**Note:**
    Maximum size limit for binary files is 100 MB."
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/which-brewing-fits-you-1080px.jpg:
    post:
      summary: Upload a binary file
      description: "Add a new file. The uploaded file will not be visible in the Kentico
        Cloud UI unless there is an asset using it, see how to [add an asset](https://developer.kenticocloud.com/v1/reference#content-management-api-add-asset).\r\n\r\n**Note:**
        Maximum size limit for binary files is 100 MB."
      operationId: FilesWhichBrewingFitsYou1080pxJpgPost
      x-api-path-slug: fileswhichbrewingfitsyou1080px-jpg-post
      parameters:
      - in: header
        name: Content-Length
        description: Specifies the size of the binary file in bytes
      - in: header
        name: Content-Type
        description: Specifies the media type of the binary data
      - in: formData
        name: File
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Binary
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