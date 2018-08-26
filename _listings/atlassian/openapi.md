---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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
---