---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get file info for post
  description: |-
    Gets a list of file information objects for the files attached to a post.
    ##### Permissions
    Must have `read_channel` permission for the channel the post is in.
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