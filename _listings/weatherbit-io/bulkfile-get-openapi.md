---
swagger: "2.0"
x-collection-name: Weatherbit.io
x-complete: 0
info:
  title: Weatherbit Get Bulk File
  description: '**(Advanced/Advanced+/Enterprise plans only)** Downloads bulk data
    files - OPTIONS: (forecast16d.json.gz - 16 day forecasts for cities > 1000 population,
    current.json.gz - Current observations for cities > 1000 population).'
  version: 2.0.0
host: api.weatherbit.io
basePath: /v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /bulk/{file}:
    get:
      summary: Get Bulk File
      description: '**(Advanced/Advanced+/Enterprise plans only)** Downloads bulk
        data files - OPTIONS: (forecast16d.json.gz - 16 day forecasts for cities >
        1000 population, current.json.gz - Current observations for cities > 1000
        population).'
      operationId: advancedadvancedenterprise-plans-only-downloads-bulk-data-files--options-forecast16djsongz--16-day-f
      x-api-path-slug: bulkfile-get
      parameters:
      - in: path
        name: file
        description: Filename (ie
      - in: query
        name: key
        description: Your registered API key
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Bulk
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