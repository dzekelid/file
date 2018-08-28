swagger: "2.0"
x-collection-name: Google Drive
x-complete: 1
info:
  title: Google Drive
  description: manages-files-in-drive-including-uploading-downloading-searching-detecting-changes-and-updating-sharing-permissions-
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /drive/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files:
    get:
      summary: Get Files
      description: Lists or searches files.
      operationId: drive.files.list
      x-api-path-slug: files-get
      parameters:
      - in: query
        name: corpora
        description: Comma-separated list of bodies of items (files/documents) to
          which the query applies
      - in: query
        name: corpus
        description: The source of files to list
      - in: query
        name: includeTeamDriveItems
        description: Whether Team Drive items should be included in results
      - in: query
        name: orderBy
        description: A comma-separated list of sort keys
      - in: query
        name: pageSize
        description: The maximum number of files to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: query
        name: q
        description: A query for filtering the file results
      - in: query
        name: spaces
        description: A comma-separated list of spaces to query within the corpus
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: teamDriveId
        description: ID of Team Drive to search
      responses:
        200:
          description: OK
      tags:
      - File
    post:
      summary: Create File
      description: Creates a new file.
      operationId: drive.files.create
      x-api-path-slug: files-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: ignoreDefaultVisibility
        description: Whether to ignore the domains default visibility settings for
          the created file
      - in: query
        name: keepRevisionForever
        description: Whether to set the keepForever field in the new head revision
      - in: query
        name: ocrLanguage
        description: A language hint for OCR processing during image import (ISO 639-1
          code)
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: useContentAsIndexableText
        description: Whether to use the uploaded content as indexable text
      responses:
        200:
          description: OK
      tags:
      - File
  /files/generateIds:
    get:
      summary: Generate File IDs
      description: Generates a set of file IDs which can be provided in create requests.
      operationId: drive.files.generateIds
      x-api-path-slug: filesgenerateids-get
      parameters:
      - in: query
        name: count
        description: The number of IDs to return
      - in: query
        name: space
        description: The space in which the IDs can be used to create new files
      responses:
        200:
          description: OK
      tags:
      - File
  /files/trash:
    delete:
      summary: Empty Trash
      description: Permanently deletes all of the user's trashed files.
      operationId: drive.files.emptyTrash
      x-api-path-slug: filestrash-delete
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{fileId}:
    delete:
      summary: Delete File
      description: Permanently deletes a file owned by the user without moving it
        to the trash. If the file belongs to a Team Drive the user must be an organizer
        on the parent. If the target is a folder, all descendants owned by the user
        are also deleted.
      operationId: drive.files.delete
      x-api-path-slug: filesfileid-delete
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      responses:
        200:
          description: OK
      tags:
      - File
    get:
      summary: Get File
      description: Gets a file's metadata or content by ID.
      operationId: drive.files.get
      x-api-path-slug: filesfileid-get
      parameters:
      - in: query
        name: acknowledgeAbuse
        description: Whether the user is acknowledging the risk of downloading known
          malware or other abusive files
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      responses:
        200:
          description: OK
      tags:
      - File
    patch:
      summary: Update File
      description: Updates a file's metadata and/or content with patch semantics.
      operationId: drive.files.update
      x-api-path-slug: filesfileid-patch
      parameters:
      - in: query
        name: addParents
        description: A comma-separated list of parent IDs to add
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: keepRevisionForever
        description: Whether to set the keepForever field in the new head revision
      - in: query
        name: ocrLanguage
        description: A language hint for OCR processing during image import (ISO 639-1
          code)
      - in: query
        name: removeParents
        description: A comma-separated list of parent IDs to remove
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      - in: query
        name: useContentAsIndexableText
        description: Whether to use the uploaded content as indexable text
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{fileId}/copy:
    post:
      summary: Copy File
      description: Creates a copy of a file and applies any requested updates with
        patch semantics.
      operationId: drive.files.copy
      x-api-path-slug: filesfileidcopy-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: ignoreDefaultVisibility
        description: Whether to ignore the domains default visibility settings for
          the created file
      - in: query
        name: keepRevisionForever
        description: Whether to set the keepForever field in the new head revision
      - in: query
        name: ocrLanguage
        description: A language hint for OCR processing during image import (ISO 639-1
          code)
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{fileId}/export:
    get:
      summary: Export File
      description: Exports a Google Doc to the requested MIME type and returns the
        exported content.
      operationId: drive.files.export
      x-api-path-slug: filesfileidexport-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: mimeType
        description: The MIME type of the format requested for this export
      responses:
        200:
          description: OK
      tags:
      - File
  /files/{fileId}/watch:
    post:
      summary: Watch File
      description: Subscribes to changes to a file
      operationId: drive.files.watch
      x-api-path-slug: filesfileidwatch-post
      parameters:
      - in: query
        name: acknowledgeAbuse
        description: Whether the user is acknowledging the risk of downloading known
          malware or other abusive files
      - in: path
        name: fileId
        description: The ID of the file
      - in: body
        name: resource
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: supportsTeamDrives
        description: Whether the requesting application supports Team Drives
      responses:
        200:
          description: OK
      tags:
      - File