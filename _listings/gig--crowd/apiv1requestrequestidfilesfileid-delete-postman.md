{
  "info": {
    "name": "GIGANDCROWD Delete Request Requestid Files Fileid",
    "_postman_id": "d216eb5c-7e4d-4f70-9dbc-b7ee78f5bdfc",
    "description": "Delete request requestid files fileid.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "3cee3902-0c5c-49b1-8b55-12f7936bc4c0",
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
              "id": "bcd00fb8-ed44-4974-909d-54b9ab15e833"
            }
          ]
        },
        {
          "id": "9c61b32a-8e76-4e17-9f5c-97b200ed209c",
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
              "id": "a319e17f-e96d-41a5-9b88-8264e3d6d933"
            }
          ]
        },
        {
          "id": "1b549c1c-628b-49e1-9016-43b4606b82c7",
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
              "id": "7f60d052-71fb-404d-8477-3c5c4c65e757"
            }
          ]
        },
        {
          "id": "da3e6220-f289-47ff-a95f-c0b3be8d6b91",
          "name": "deleteApiV1RequestRequestFilesFile",
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
            "method": "DELETE",
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
            "description": "Delete request requestid files fileid."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e53c1b9-9375-4363-8058-c54e8f2d9f28"
            }
          ]
        }
      ]
    }
  ]
}