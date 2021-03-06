---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 0
info:
  title: Google Play Decline Room
  version: 1.0.0
  description: Decline an invitation to join a room. For internal use by the Games
    SDK only. Calling this method directly is unsupported.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rooms:
    get:
      summary: Get Rooms
      description: Returns invitations to join rooms.
      operationId: games.rooms.list
      x-api-path-slug: rooms-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: query
        name: maxResults
        description: The maximum number of rooms to return in the response, used for
          paging
      - in: query
        name: pageToken
        description: The token returned by the previous request
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/create:
    post:
      summary: Create Room
      description: Create a room. For internal use by the Games SDK only. Calling
        this method directly is unsupported.
      operationId: games.rooms.create
      x-api-path-slug: roomscreate-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}:
    get:
      summary: Get Room
      description: Get the data for a room.
      operationId: games.rooms.get
      x-api-path-slug: roomsroomid-get
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/decline:
    post:
      summary: Decline Room
      description: Decline an invitation to join a room. For internal use by the Games
        SDK only. Calling this method directly is unsupported.
      operationId: games.rooms.decline
      x-api-path-slug: roomsroomiddecline-post
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: query
        name: language
        description: The preferred language to use for strings returned by this method
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
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