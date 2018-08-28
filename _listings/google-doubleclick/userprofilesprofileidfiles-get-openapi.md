---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Files
  version: 1.0.0
  description: Lists files for a user profile.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/files:
    get:
      summary: Get Files
      description: Lists files for a user profile.
      operationId: dfareporting.files.list
      x-api-path-slug: userprofilesprofileidfiles-get
      parameters:
      - in: query
        name: maxResults
        description: Maximum number of results to return
      - in: query
        name: pageToken
        description: The value of the nextToken from the previous result page
      - in: path
        name: profileId
        description: The DFA profile ID
      - in: query
        name: scope
        description: The scope that defines which results are returned, default is
          MINE
      - in: query
        name: sortField
        description: The field by which to sort the list
      - in: query
        name: sortOrder
        description: Order of sorted results, default is DESCENDING
      responses:
        200:
          description: OK
      tags:
      - Advertising
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