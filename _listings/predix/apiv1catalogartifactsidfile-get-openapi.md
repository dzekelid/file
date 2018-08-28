---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Framework Download an artifact file by id.
  version: 1.0.0
  description: The file is downloaded as an octet-stream.
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/catalog/artifacts/{id}/file:
    get:
      summary: Download an artifact file by id.
      description: The file is downloaded as an octet-stream.
      operationId: downloadAnalyticArtifact
      x-api-path-slug: apiv1catalogartifactsidfile-get
      parameters:
      - in: path
        name: id
        description: artifact id
      responses:
        2:
          description: Successful response
      tags:
      - Download
      - Artifact
      - File
      - By
      - Id
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