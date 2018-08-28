---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Attaches an externally hosted document to a room within a room description.
  version: 1.0.0
  description: Attaches an externally hosted document to a room within a room description..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/room/{id}:
    get:
      summary: Get a room by its Id
      description: Get a room by its id.
      operationId: Room_GetByid
      x-api-path-slug: apiroomid-get
      parameters:
      - in: path
        name: id
        description: The id of the room to get
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Room
      - By
      - Its
      - Id
  /api/roomdescription/{id}/attachexternaldocumenttoroom:
    put:
      summary: Attaches an externally hosted document to a room within a room description.
      description: Attaches an externally hosted document to a room within a room
        description..
      operationId: RoomDescription_AttachExternalDocumentToRoomByidByexternalDocumentByroomId
      x-api-path-slug: apiroomdescriptionidattachexternaldocumenttoroom-put
      parameters:
      - in: body
        name: externalDocument
        description: Details of the external document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The RoomDescriptionId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The room identifier
      responses:
        200:
          description: OK
      tags:
      - Attaches
      - Externally
      - Hosted
      - Document
      - To
      - Room
      - Within
      - Room
      - Description
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