swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 1
info:
  title: Kentico Cloud
  description: this-is-a-collection-of-resources-you-can-find-within-the-kentico-cloud-developer-hubhttpsdeveloper-kenticocloud-com--kentico-cloudhttpskenticocloud-com-is-a-cloudfirst-headless-cms-that-allows-you-to-distribute-content-to-any-channel-and-device-websites-mobile-devices-mixed-reality-devices-presentation-kiosks-etc--through-an-api-certain-apis-require-that-you-include-the-authorization-header--find-more-in-httpsdeveloper-kenticocloud-comreferenceauthentication-
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/which-brewing-fits-you-1080px.jpg:
    post:
      summary: Upload a binary file
      description: "Add a new file. The uploaded file will not be visible in the Kentico
        Cloud UI unless there is an asset using it, see how to [add an asset](https://developer.kenticocloud.com/v1/reference#content-management-api-add-asset).\r\n\r\n**Note:**
        Maximum size limit for binary files is 100 MB."
      operationId: FilesWhichBrewingFitsYou1080pxJpgPost
      x-api-path-slug: fileswhichbrewingfitsyou1080px-jpg-post
      parameters:
      - in: header
        name: Content-Length
        description: Specifies the size of the binary file in bytes
      - in: header
        name: Content-Type
        description: Specifies the media type of the binary data
      - in: formData
        name: File
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Binary
      - File