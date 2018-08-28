{
  "info": {
    "name": "GIGANDCROWD Get Request Requestid Files Fileid",
    "_postman_id": "e9408633-c39a-42f2-b11b-ed11b4744362",
    "description": "Get request requestid files fileid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "e8a2e745-db53-4b37-8145-ecc23c95877b",
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
              "id": "4be1f6c7-2327-4d27-a34c-c2eba03be84f"
            }
          ]
        },
        {
          "id": "8d11679f-9026-429a-95c2-6d14d0be75cf",
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
              "id": "b05be126-de08-4129-b564-b1f1974b6589"
            }
          ]
        },
        {
          "id": "8df16d8e-3138-4e47-bb69-fb94df61356a",
          "name": "getApiV1RequestRequestFilesFile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/request/:requestId/files/:fileId"
              ],
              "variable": [
                {
                  "id": "fileId",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Get request requestid files fileid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ede8e357-d4fa-4ef2-9888-e9a35d13ab08"
            }
          ]
        }
      ]
    }
  ]
}