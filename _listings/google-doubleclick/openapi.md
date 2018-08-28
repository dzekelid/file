swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 1
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
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