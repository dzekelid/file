swagger: "2.0"
x-collection-name: Weatherbit.io
x-complete: 1
info:
  title: Weatherbit
  description: this-is-the-documentation-for-the-weatherbit-api---the-base-url-for-the-api-is-httpapi-weatherbit-iov2-0httpapi-weatherbit-iov2-0-or-httpsapi-weatherbit-iov2-0httpapi-weatherbit-iov2-0--below-is-the-swagger-ui-documentation-for-the-api--all-api-requests-require-the-key-parameter---------an-example-for-a-5-day-forecast-for-london-uk-would-be-httpapi-weatherbit-iov2-0forecast3hourlycitylondoncountryuk
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