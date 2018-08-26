---
swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 0
info:
  title: Ge.tt  REST API Files  Upload
  description: Get upload urls to the file. This returns a new PUT and POST url for
    you to upload the file to.nOBS You can also choose to use the put- or posturl
    that you were previously given to override the file.
  termsOfService: http://ge.tt/terms
  version: "1"
host: open.ge.tt
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1/files/{sharename}/create:
    post:
      summary: Files Create
      description: 'To upload files to Ge.tt you must first create the file under
        a given share. You do that by posting the filename:'
      operationId: post1FilesSharenameCreate
      x-api-path-slug: 1filessharenamecreate-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Create
  /1/files/{sharename}/{fileid}:
    get:
      summary: Files
      description: 'Get the state of a file. This returns the following data:'
      operationId: get1FilesSharenameFile
      x-api-path-slug: 1filessharenamefileid-get
      parameters:
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
  /1/files/{sharename}/{fileid}/blob:
    get:
      summary: Files  Blob
      description: Will redirect to the binary content of the file
      operationId: get1FilesSharenameFileBlob
      x-api-path-slug: 1filessharenamefileidblob-get
      parameters:
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Blob
  /1/files/{sharename}/{fileid}/blob/thumb:
    get:
      summary: Files  Blob Thumb
      description: Will redirect to a thumbnail of the binary file. Currently only
        available for images.
      operationId: get1FilesSharenameFileBlobThumb
      x-api-path-slug: 1filessharenamefileidblobthumb-get
      parameters:
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Blob
      - Thumb
  /1/files/{sharename}/{fileid}/destroy:
    post:
      summary: Files  Destroy
      description: Delete a file and the binary contents.
      operationId: post1FilesSharenameFileDestroy
      x-api-path-slug: 1filessharenamefileiddestroy-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Destroy
  /1/files/{sharename}/{fileid}/upload:
    get:
      summary: Files  Upload
      description: Get upload urls to the file. This returns a new PUT and POST url
        for you to upload the file to.nOBS You can also choose to use the put- or
        posturl that you were previously given to override the file.
      operationId: get1FilesSharenameFileUpload
      x-api-path-slug: 1filessharenamefileidupload-get
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: fileid
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Files
      - Sharename
      - Fileid
      - Upload
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