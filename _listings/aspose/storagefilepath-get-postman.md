{
  "info": {
    "name": "Aspose.Storage API Get Storage File Path",
    "_postman_id": "1a63f1ba-7e5b-4710-8969-c69b5d169bb1",
    "description": "The resource represents customers file at server file storage.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Storage",
      "item": [
        {
          "id": "c67b783f-5b07-4a0e-84d9-8bfc9e1cb3f2",
          "name": "getStorageDisc",
          "request": {
            "url": "http://api.aspose.com/v1.1/storage/disc",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The resource represents information about users application disc usage (size in bytes"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4bd56e4b-4378-43e6-94d4-a9ca1ec15f6f"
            }
          ]
        },
        {
          "id": "635bf1e3-136b-4c2c-93d5-86fc2e262f52",
          "name": "getStorageExistPath",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.aspose.com",
              "path": [
                "v1.1",
                "storage/exist/:path"
              ],
              "variable": [
                {
                  "id": "path",
                  "value": "path",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The controller checks that the file or folder exists in the service file storage."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed6db079-188c-4611-86e8-4f8470df1912"
            }
          ]
        },
        {
          "id": "3a73a3b7-e407-43d5-b397-bd91f45dfb3d",
          "name": "getStorageFilePath",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.aspose.com",
              "path": [
                "v1.1",
                "storage/file/:path"
              ],
              "variable": [
                {
                  "id": "path",
                  "value": "path",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The resource represents customers file at server file storage."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7951f064-25e6-473a-8fb5-12c46b0c8f9b"
            }
          ]
        },
        {
          "id": "34222b04-a4d3-4918-a2ae-bed16a6a5cab",
          "name": "deleteStorageFilePath",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.aspose.com",
              "path": [
                "v1.1",
                "storage/file/:path"
              ],
              "variable": [
                {
                  "id": "path",
                  "value": "path",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "The resource represents customers file at server file sto"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc61de2c-3578-4b6b-bf76-10adbdda30e1"
            }
          ]
        }
      ]
    }
  ]
}