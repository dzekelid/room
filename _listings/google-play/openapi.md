---
swagger: "2.0"
x-collection-name: Google Play
x-complete: 1
info:
  title: Google Play
  version: 1.0.0
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
  /rooms/{roomId}/dismiss:
    post:
      summary: Dismiss Room
      description: Dismiss an invitation to join a room. For internal use by the Games
        SDK only. Calling this method directly is unsupported.
      operationId: games.rooms.dismiss
      x-api-path-slug: roomsroomiddismiss-post
      parameters:
      - in: query
        name: consistencyToken
        description: The last-seen mutation timestamp
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/join:
    post:
      summary: Join Room
      description: Join a room. For internal use by the Games SDK only. Calling this
        method directly is unsupported.
      operationId: games.rooms.join
      x-api-path-slug: roomsroomidjoin-post
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
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/leave:
    post:
      summary: Leave Room
      description: Leave a room. For internal use by the Games SDK only. Calling this
        method directly is unsupported.
      operationId: games.rooms.leave
      x-api-path-slug: roomsroomidleave-post
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
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
  /rooms/{roomId}/reportstatus:
    post:
      summary: Report Room Status
      description: Updates sent by a client reporting the status of peers in a room.
        For internal use by the Games SDK only. Calling this method directly is unsupported.
      operationId: games.rooms.reportStatus
      x-api-path-slug: roomsroomidreportstatus-post
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
      - in: path
        name: roomId
        description: The ID of the room
      responses:
        200:
          description: OK
      tags:
      - Room
---