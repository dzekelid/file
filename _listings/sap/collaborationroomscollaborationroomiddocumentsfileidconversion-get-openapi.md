---
swagger: "2.0"
x-collection-name: SAP
x-complete: 0
info:
  title: SAP Manufacturing Network Customer APIs Gets conversion info of a design
    file
  description: "Retrieves the information of the conversion event for a design file.\nA
    conversion event converts a design file into a VDS file.  \nSee a full list of
    supported formats in the [online help](https://help.sap.com/viewer/dmc-mn-app-help-customer/710ee60457ca457cbda854c363bcf71f.html)."
  version: 1.0.0
host: hostname
basePath: /dim/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /collaborationRooms/{collaborationRoomId}/documents/{fileId}/conversion:
    get:
      summary: Gets conversion info of a design file
      description: "Retrieves the information of the conversion event for a design
        file.\nA conversion event converts a design file into a VDS file.  \nSee a
        full list of supported formats in the [online help](https://help.sap.com/viewer/dmc-mn-app-help-customer/710ee60457ca457cbda854c363bcf71f.html)."
      operationId: retrieves-the-information-of-the-conversion-event-for-a-design-filea-conversion-event-converts-a-des
      x-api-path-slug: collaborationroomscollaborationroomiddocumentsfileidconversion-get
      parameters:
      - in: path
        name: collaborationRoomId
        description: The ID of a collaboration room
      - in: path
        name: fileId
        description: The ID of a file
      responses:
        200:
          description: Successful response
      tags:
      - S
      - Conversion
      - Info
      - Of
      - Design
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