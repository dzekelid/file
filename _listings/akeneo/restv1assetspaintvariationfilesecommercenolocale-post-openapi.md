---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API asset variation file (2.1 only)
  description: Assuming that the given codes are respectively the code of an existing
    asset, an existing channel and an activated locale if the asset is localizable
    (it should be equal to "no-locale" otherwise)
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
    post:
      summary: asset reference file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset and an activated locale if the asset is localizable (it should be equal
        to "no-locale" otherwise)
      operationId: RestV1AssetsPaintReferenceFilesNoLocalePost
      x-api-path-slug: restv1assetspaintreferencefilesnolocale-post
      parameters:
      - in: header
        name: Content-Type
      - in: formData
        name: file
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
  /rest/v1/assets/paint/reference-files/no-locale/download:
    get:
      summary: download asset reference file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset and an activated locale if the asset is localizable (it should be equal
        to "no-locale" otherwise)
      operationId: RestV1AssetsPaintReferenceFilesNoLocaleDownloadGet
      x-api-path-slug: restv1assetspaintreferencefilesnolocaledownload-get
      responses:
        200:
          description: OK
      tags:
      - Download
      - Asset
      - Reference
      - File
      - (2
      - "1"
      - Only)
  /rest/v1/assets/paint/variation-files/ecommerce/no-locale:
    get:
      summary: asset variation file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset, an existing channel and an activated locale if the asset is localizable
        (it should be equal to "no-locale" otherwise)
      operationId: RestV1AssetsPaintVariationFilesEcommerceNoLocaleGet
      x-api-path-slug: restv1assetspaintvariationfilesecommercenolocale-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Variation
      - File
      - (2
      - "1"
      - Only)
    post:
      summary: asset variation file (2.1 only)
      description: Assuming that the given codes are respectively the code of an existing
        asset, an existing channel and an activated locale if the asset is localizable
        (it should be equal to "no-locale" otherwise)
      operationId: RestV1AssetsPaintVariationFilesEcommerceNoLocalePost
      x-api-path-slug: restv1assetspaintvariationfilesecommercenolocale-post
      parameters:
      - in: header
        name: Content-Type
      - in: formData
        name: file
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Variation
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