---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Software Cloud API Upload a file
  description: Authentication required, with scope participate:conversation
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/{conversationId}/media:
    post:
      summary: Upload a file
      description: Authentication required, with scope participate:conversation
      operationId: ConversationMediaPostHandler
      x-api-path-slug: sitecloudidconversationconversationidmedia-post
      parameters:
      - in: path
        name: cloudId
        description: Cloud ID
      - in: path
        name: conversationId
        description: Conversation ID
      - in: query
        name: name
        description: File name
      responses:
        200:
          description: OK
      tags:
      - Upload
      - File
  /site/{cloudId}/conversation/{conversationId}/media/{mediaId}:
    get:
      summary: Get a file
      description: Authentication required, with scope participate:conversation
      operationId: ConversationMediaGetHandler
      x-api-path-slug: sitecloudidconversationconversationidmediamediaid-get
      parameters:
      - in: path
        name: cloudId
        description: Cloud ID
      - in: path
        name: conversationId
        description: Conversation ID
      - in: path
        name: mediaId
        description: Media ID
      responses:
        200:
          description: OK
      tags:
      - File
    delete:
      summary: Delete a file
      description: Authentication required, with scope participate:conversation
      operationId: ConversationMediaDeleteHandler
      x-api-path-slug: sitecloudidconversationconversationidmediamediaid-delete
      parameters:
      - in: path
        name: cloudId
        description: Cloud ID
      - in: path
        name: conversationId
        description: Conversation ID
      - in: path
        name: mediaId
        description: Media ID
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