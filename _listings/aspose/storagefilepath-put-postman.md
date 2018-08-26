{
  "info": {
    "name": "Aspose.Storage API Put Storage File Path",
    "_postman_id": "adc3a789-7e0e-443e-9153-9016bcd6345f",
    "description": "The resource represents customers file at server file storage.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Storage",
      "item": [
        {
          "id": "236ccc5b-44b5-4282-8c66-426081f9e4eb",
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
              "id": "f9f0bbd5-d9a6-4f85-85bc-2709d2299955"
            }
          ]
        },
        {
          "id": "db6ebc0a-840b-44a7-a95d-5311eadeef1f",
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
              "id": "0a40f53b-4b43-47a7-bf8c-09bce7952cd2"
            }
          ]
        },
        {
          "id": "13477d3b-5140-4334-9852-c9f8ce83cf1b",
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
              "id": "e2288752-01d8-471c-95a9-247490560ae5"
            }
          ]
        },
        {
          "id": "4ccb2312-d11d-4dbd-9401-9354b6c786d9",
          "name": "putStorageFilePath",
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
            "method": "PUT",
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
              "id": "79b89e3b-f324-45ba-8c9a-410df92175a9"
            }
          ]
        },
        {
          "id": "91af6742-5a02-4027-ac1b-d1797b5ebf13",
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
              "id": "ef933d1d-bd19-462b-aefa-a9150388f6e2"
            }
          ]
        },
        {
          "id": "772f0c9f-d6fc-466e-9df1-e6360dea3695",
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
              "id": "0f29312f-aa4d-43f3-aa6b-6281291783b9"
            }
          ]
        }
      ]
    }
  ]
}