---
swagger: "2.0"
x-collection-name: TelAPI
x-complete: 0
info:
  title: hetras Hotel API Version 0 Get all the details for a specific room type in
    the hotel.
  version: v0
  description: With this call you can load the details about a specific room type
    in the hotel.
host: api.hetras-certification.net
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/hotel/v0/hotels/{hotelId}/room_types:
    get:
      summary: Get a list with the details of all room types for for the specified
        hotel id.
      description: With this call you can load the details about a all available room
        types for the specified hotel.
      operationId: RoomTypes_GetRoomTypes
      x-api-path-slug: apihotelv0hotelshotelidroom-types-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the room type belongs to
      responses:
        200:
          description: OK
      tags:
      - List
      - Details
      - Of
      - ""
      - Room
      - Typesfor
      - Specified
      - Hotel
      - Id
  /api/hotel/v0/hotels/{hotelId}/room_types/{code}:
    get:
      summary: Get all the details for a specific room type in the hotel.
      description: With this call you can load the details about a specific room type
        in the hotel.
      operationId: RoomTypes_GetRoomType
      x-api-path-slug: apihotelv0hotelshotelidroom-typescode-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: code
        description: The code of the room type you want to see details for
      - in: path
        name: hotelId
        description: The hotel id the room type belongs to
      responses:
        200:
          description: OK
      tags:
      - Detailsa
      - Specific
      - Room
      - Type
      - In
      - Hotel
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