---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API asset reference file (2.1 only)
  description: Assuming that the given codes are respectively the code of an existing
    asset and an activated locale if the asset is localizable (it should be equal
    to "no-locale" otherwise)
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/assets/paint/reference-files/no-locale:
    get:
      summary: asset reference file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset and an activated locale if the asset is localizable (it should be equal
        to "no-locale" otherwise)
      operationId: RestV1AssetsPaintReferenceFilesNoLocaleGet
      x-api-path-slug: restv1assetspaintreferencefilesnolocale-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Reference
      - File
      - (2
      - "1"
      - Only)
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