---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Remove license file
  description: |-
    Remove the license file from the server. This will disable all enterprise features.

    __Minimum server version__: 4.0

    ##### Permissions
    Must have `manage_system` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /posts/{post_id}/files/info:
    get:
      summary: Get file info for post
      description: |-
        Gets a list of file information objects for the files attached to a post.
        ##### Permissions
        Must have `read_channel` permission for the channel the post is in.
      operationId: gets-a-list-of-file-information-objects-for-the-files-attached-to-a-post-permissionsmust-have-read-c
      x-api-path-slug: postspost-idfilesinfo-get
      parameters:
      - in: path
        name: post_id
        description: ID of the post
      responses:
        200:
          description: OK
      tags:
      - File
      - Infopost
  /files:
    post:
      summary: Upload a file
      description: |-
        Uploads a file that can later be attached to a post.

        This request can either be a multipart/form-data request with a channel_id, files and optional
        client_ids defined in the FormData, or it can be a request with the channel_id and filename
        defined as query parameters with the contents of a single file in the body of the request.

        Only multipart/form-data requests are supported by server versions up to and including 4.7.
        Server versions 4.8 and higher support both types of requests.

        ##### Permissions
        Must have `upload_file` permission.
      operationId: uploads-a-file-that-can-later-be-attached-to-a-postthis-request-can-either-be-a-multipartformdata-re
      x-api-path-slug: files-post
      parameters:
      - in: formData
        name: channel_id
        description: The ID of the channel that this file will be uploaded to
      - in: query
        name: channel_id
        description: The ID of the channel that this file will be uploaded to
      - in: formData
        name: client_ids
        description: A unique identifier for the file that will be returned in the
          response
      - in: query
        name: filename
        description: The ID of the channel that this file will be uploaded to
      - in: formData
        name: files
        description: A file to be uploaded
      responses:
        200:
          description: OK
      tags:
      - Upload
      - File
  /files/{file_id}:
    get:
      summary: Get a file
      description: |-
        Gets a file that has been uploaded previously.
        ##### Permissions
        Must have `read_channel` permission or be uploader of the file.
      operationId: gets-a-file-that-has-been-uploaded-previously-permissionsmust-have-read-channel-permission-or-be-upl
      x-api-path-slug: filesfile-id-get
      parameters:
      - in: path
        name: file_id
        description: The ID of the file to get
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{file_id}/link:
    get:
      summary: Get a public file link
      description: Gets a public link for a file that can be accessed without logging
        into Mattermost.
      operationId: gets-a-public-link-for-a-file-that-can-be-accessed-without-logging-into-mattermost
      x-api-path-slug: filesfile-idlink-get
      parameters:
      - in: path
        name: file_id
        description: The ID of the file to get a link for
      responses:
        200:
          description: OK
      tags:
      - Public
      - File
      - Link
  /files/{file_id}/info:
    get:
      summary: Get metadata for a file
      description: |-
        Gets a file's info.
        ##### Permissions
        Must have `read_channel` permission or be uploader of the file.
      operationId: gets-a-files-info-permissionsmust-have-read-channel-permission-or-be-uploader-of-the-file
      x-api-path-slug: filesfile-idinfo-get
      parameters:
      - in: path
        name: file_id
        description: The ID of the file info to get
      responses:
        200:
          description: OK
      tags:
      - Metadataa
      - File
  /license:
    post:
      summary: Upload license file
      description: |-
        Upload a license to enable enterprise features.

        __Minimum server version__: 4.0

        ##### Permissions
        Must have `manage_system` permission.
      operationId: upload-a-license-to-enable-enterprise-features-minimum-server-version--40-permissionsmust-have-manag
      x-api-path-slug: license-post
      parameters:
      - in: formData
        name: license
        description: The license to be uploaded
      responses:
        200:
          description: OK
      tags:
      - Upload
      - License
      - File
    delete:
      summary: Remove license file
      description: |-
        Remove the license file from the server. This will disable all enterprise features.

        __Minimum server version__: 4.0

        ##### Permissions
        Must have `manage_system` permission.
      operationId: remove-the-license-file-from-the-server-this-will-disable-all-enterprise-features-minimum-server-ver
      x-api-path-slug: license-delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - License
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