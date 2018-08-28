swagger: "2.0"
x-collection-name: GlobalChange.gov
x-complete: 1
info:
  title: Global Change Information System API
  description: who-we-are-what-the-gcis-is-and-how-we-use-identifiers-and-semantic-information-to-provide-points-of-reference-and-traceability--examples-and-tutorials-for-using-this-system-as-a-researcher-citizen-scientist-application-developer-or-information-theorist--a-description-of-how-the-information-is-structured-including-the-overlaps-between-relational-and-semantic-representations-of-the-information--complete-documentation-for-the-api-including-methods-for-browsing-and-finding-resources-
  version: v1
host: data.globalchange.gov
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /file/{file_identifier}:
    get:
      summary: Get a representation of a file.
      description: Get JSON which represents the structure of a file.
      operationId: get-json-which-represents-the-structure-of-a-file
      x-api-path-slug: filefile-identifier-get
      parameters:
      - in: path
        name: file_identifier
        description: file_identifier description
      responses:
        200:
          description: OK
      tags:
      - Representation
      - File