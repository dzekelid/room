{
  "info": {
    "name": "Dezrez Get a room by its Id",
    "_postman_id": "b175c7dc-b79f-4aef-8021-69866c950f2a",
    "description": "Get a room by its id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Room",
      "item": [
        {
          "id": "a25a61b4-1014-423d-9f67-6778dd9ba9bd",
          "name": "Room_GetByid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/room/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a room by its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "098c797b-4810-4fe8-ad57-ac78f771b11d"
            }
          ]
        }
      ]
    }
  ]
}