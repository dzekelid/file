---
swagger: "2.0"
x-collection-name: Google Drive
x-complete: 0
info:
  title: Google Drive Get Files
  description: Lists or searches files.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /drive/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files:
    get:
      summary: Get Files
      description: Lists or searches files.
      operationId: drive.files.list
      x-api-path-slug: files-get
      parameters:
      - in: query
        name: corpora
        description: Comma-separated list of bodies of items (files/documents) to
          which the query applies
      - in: query
        name: corpus
        description: The source of files to list
      - in: query
        name: includeTeamDriveItems
        description: Whether Team Drive items should be included in results
      - in: query
        name: orderBy
        description: A comma-separated list of sort keys
      - in: query
        name: pageSize
        description: The maximum number of files to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: query
        name: q
        description: A query for filtering the file results
      - in: query
        name: spaces
        description: A comma-separated list of spaces to query within the corpus
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: teamDriveId
        description: ID of Team Drive to search
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