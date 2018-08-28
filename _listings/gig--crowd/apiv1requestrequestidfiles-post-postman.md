{
  "info": {
    "name": "GIGANDCROWD Post Request Requestid Files",
    "_postman_id": "6e235dc1-75f0-4a37-bba8-24df28cfa716",
    "description": "Post request requestid files.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "dfee935b-0c9f-410f-8361-b18a9f88b929",
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
              "id": "0710f9e0-23d8-44c2-b1e4-23fab7c9c509"
            }
          ]
        },
        {
          "id": "654c106d-9915-40d5-9e25-a9c99640891d",
          "name": "postApiV1RequestRequestFiles",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/request/:requestId/files"
              ],
              "query": [
                {
                  "key": "file",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "requestId",
                  "value": "requestId",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
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
            "description": "Post request requestid files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "860425bf-22dd-46b9-b7e6-ae0f288481ad"
            }
          ]
        }
      ]
    }
  ]
}