swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateNFSFileShare:
    get:
      summary: Create NFS File Share
      description: Creates a file share on an existing file gateway.
      operationId: createNFSFileShare
      x-api-path-slug: actioncreatenfsfileshare-get
      parameters:
      - in: query
        name: ClientToken
        description: A unique string value that you supply that is used by file gateway
          to ensure         idempotent file share creation
        type: string
      - in: query
        name: DefaultStorageClass
        description: The default storage class for objects put into an Amazon S3 bucket
          by file gateway
        type: string
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the file gateway on which you
          want to create a file share
        type: string
      - in: query
        name: KMSEncrypted
        description: True to use Amazon S3 server side encryption with your own AWS
          KMS key, or false to         use a key managed by Amazon S3
        type: string
      - in: query
        name: KMSKey
        description: The KMS key used for Amazon S3 server side encryption
        type: string
      - in: query
        name: LocationARN
        description: The ARN of the backend storage used for storing file data
        type: string
      - in: query
        name: NFSFileShareDefaults
        description: File share default values
        type: string
      - in: query
        name: Role
        description: The ARN of the AWS Identity and Access Management (IAM) role
          that a file gateway         assumes when it accesses the underlying storage
        type: string
      responses:
        200:
          description: OK
      tags:
      - NFS File Share
  /?Action=DeleteFileShare:
    get:
      summary: Delete File Share
      description: Deletes a file share from a file gateway.
      operationId: deleteFileShare
      x-api-path-slug: actiondeletefileshare-get
      parameters:
      - in: query
        name: FileShareARN
        description: The Amazon Resource Name (ARN) of the file share to be deleted
        type: string
      responses:
        200:
          description: OK
      tags:
      - File Share
  /?Action=DescribeNFSFileShares:
    get:
      summary: Describe NFS File Shares
      description: Gets a description for one or more file shares from a file gateway.
      operationId: describeNFSFileShares
      x-api-path-slug: actiondescribenfsfileshares-get
      parameters:
      - in: query
        name: FileShareARNList
        description: An array containing the Amazon Resource Name (ARN) of each file
          share to be described
        type: string
      responses:
        200:
          description: OK
      tags:
      - NFS File Shares
  /?Action=ListFileShares:
    get:
      summary: List File Shares
      description: Gets a list of the file shares for a specific file gateway, or
        the list of file shares that belong to the calling user account.
      operationId: listFileShares
      x-api-path-slug: actionlistfileshares-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon resource Name (ARN) of the gateway whose file shares
          you want to list
        type: string
      - in: query
        name: Limit
        description: The maximum number of file shares to return in the response
        type: string
      - in: query
        name: Marker
        description: Opaque pagination token returned from a previous ListFileShares
          operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - File Shares
  /?Action=UpdateNFSFileShare:
    get:
      summary: Update NFS File Share
      description: Updates a file share.
      operationId: updateNFSFileShare
      x-api-path-slug: actionupdatenfsfileshare-get
      parameters:
      - in: query
        name: DefaultStorageClass
        description: The default storage class for objects put into an Amazon S3 bucket
          by a file gateway
        type: string
      - in: query
        name: FileShareARN
        description: The Amazon Resource Name (ARN) of the file share to be updated
        type: string
      - in: query
        name: KMSEncrypted
        description: True to use Amazon S3 server side encryption with your own AWS
          KMS key, or false to         use a key managed by Amazon S3
        type: string
      - in: query
        name: KMSKey
        description: The KMS key used for Amazon S3 server side encryption
        type: string
      - in: query
        name: NFSFileShareDefaults
        description: The default values for the file share
        type: string
      responses:
        200:
          description: OK
      tags:
      - NFS File Share