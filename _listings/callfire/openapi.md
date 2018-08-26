---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /media/{id}/file:
    get:
      summary: Download a MP3 media
      description: Download a MP3 media, endpoint returns application/binary content-type
      operationId: getMediaDataBinary
      x-api-path-slug: mediaidfile-get
      parameters:
      - in: path
        name: id
        description: An id of a media resource
      responses:
        200:
          description: OK
      tags:
      - Media
      - File
---