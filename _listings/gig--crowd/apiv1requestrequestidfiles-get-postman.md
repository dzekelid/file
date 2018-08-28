{
  "info": {
    "name": "GIGANDCROWD Get Request Requestid Files",
    "_postman_id": "d3a63a67-d477-4dff-9cd8-5b8ed5f3f373",
    "description": "Get request requestid files.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "cd503364-1857-4a8e-a466-236b7e3d97ae",
          "name": "getApiV1RequestRequestFiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/request/:requestId/files"
              ],
              "variable": [
                {
                  "id": "requestId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "",
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
            "description": "Get request requestid files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "803ecf4d-e4aa-4f87-911d-0fd9dcfe11c3"
            }
          ]
        }
      ]
    }
  ]
}