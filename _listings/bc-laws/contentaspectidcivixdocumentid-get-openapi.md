---
swagger: "2.0"
x-collection-name: BC Laws
x-complete: 0
info:
  title: BC Laws Lists the metadata available for the specified index or directory
    from the BCLaws legislative respository
  description: Lists the metadata available for the specified index or directory from
    the BCLaws legislative respository
  termsOfService: http://www.data.gov.bc.ca/local/dbc/docs/license/API_Terms_of_Use.pdf
  version: 1.0.0
host: www.bclaws.ca
basePath: /civix
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /content/{aspectId}:
    get:
      summary: Describes the documents and directories available within a specific
        'aspect' (content group) of the BCLaws library
      description: Describes the documents and directories available within a specific
        'aspect' (content group) of the BCLaws library
      operationId: getContentAspect
      x-api-path-slug: contentaspectid-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      responses:
        200:
          description: OK
      tags:
      - Content
      - AspectId
  /content/{aspectId}/{civixDocumentId}:
    get:
      summary: Lists the metadata available for the specified index or directory from
        the BCLaws legislative respository
      description: Lists the metadata available for the specified index or directory
        from the BCLaws legislative respository
      operationId: getContentAspectCivixdocument
      x-api-path-slug: contentaspectidcivixdocumentid-get
      parameters:
      - in: path
        name: aspectId
        description: The identifier of the aspect (content group) to search
      - in: path
        name: civixDocumentId
        description: The document identification code for an index or directory
      responses:
        200:
          description: OK
      tags:
      - Content
      - AspectId
      - CivixDocumentId
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