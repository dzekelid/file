swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/glip/files:
    post:
      summary: Upload File
      description: |-
        Posts a file.
        App Permission
        Glip
        User Permission
        Glip
        Usage Plan Group
        Heavy
      operationId: createGlipFile
      x-api-path-slug: restapiv1-0glipfiles-post
      parameters:
      - in: formData
        name: body
        description: The file to upload
      - in: query
        name: groupId
        description: Internal identifier of a group to which the post with attachement
          will be added to
      - in: formData
        name: name
        description: Name of a file attached
      responses:
        200:
          description: OK
      tags:
      - Upload
      - File