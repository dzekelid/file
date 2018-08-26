{
  "info": {
    "name": "Aspose.Storage API Post Storage File Path",
    "_postman_id": "e5616802-4c94-4548-a19a-9da0cc1c874b",
    "description": "The resource represents customers file at server file storage",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Storage",
      "item": [
        {
          "id": "e608f944-859e-4093-93ce-5f1a80e1da11",
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
              "id": "2568de60-a1dd-42ce-9529-8c814bccad33"
            }
          ]
        },
        {
          "id": "d61f1478-f602-4a9c-a17e-bdda483b1f9e",
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
              "id": "892e5d71-4f03-491f-bd57-062ff9297e70"
            }
          ]
        },
        {
          "id": "682d9dcb-3ebd-4dbd-bf15-966dc630d02c",
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
              "id": "41543569-bd5a-4a50-9d36-d0f80518bd66"
            }
          ]
        },
        {
          "id": "f4d0590e-321c-4324-9896-0c1c8111e14f",
          "name": "postStorageFilePath",
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "The resource represents customers file at server file storage"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "adaa1e73-3f96-40f8-bbf1-2c329e61f084"
            }
          ]
        },
        {
          "id": "8303ac06-e4a1-4316-9df8-f8a135475c0c",
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
              "id": "a28a21f4-3c7e-4728-8b79-4c1603e19458"
            }
          ]
        }
      ]
    }
  ]
}