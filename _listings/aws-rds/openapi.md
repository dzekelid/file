swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeDBLogFiles:
    get:
      summary: Describe D B Log Files
      description: Returns a list of DB log files for the DB instance.
      operationId: describedblogfiles
      x-api-path-slug: actiondescribedblogfiles-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The customer-assigned name of the DB instance that contains the
          log files you want to list
        type: string
      - in: query
        name: FileLastWritten
        description: Filters the available log files for files written since the specified
          date, in POSIX timestamp format with milliseconds
        type: string
      - in: query
        name: FilenameContains
        description: Filters the available log files for log file names that contain
          the specified string
        type: string
      - in: query
        name: FileSize
        description: Filters the available log files for files larger than the specified
          size
        type: string
      - in: query
        name: Filters.Filter.N
        description: This parameter is not currently supported
        type: string
      - in: query
        name: Marker
        description: The pagination token provided in the previous request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - Blog Files
  /?Action=DownloadDBLogFilePortion:
    get:
      summary: Download D B Log File Portion
      description: Downloads all or a portion of the specified log file, up to 1 MB
        in size.
      operationId: downloaddblogfileportion
      x-api-path-slug: actiondownloaddblogfileportion-get
      parameters:
      - in: query
        name: DBInstanceIdentifier
        description: The customer-assigned name of the DB instance that contains the
          log files you want to list
        type: string
      - in: query
        name: LogFileName
        description: The name of the log file to be downloaded
        type: string
      - in: query
        name: Marker
        description: The pagination token provided in the previous request or 0
        type: string
      - in: query
        name: NumberOfLines
        description: The number of lines to download
        type: string
      responses:
        200:
          description: OK
      tags:
      - Log Files