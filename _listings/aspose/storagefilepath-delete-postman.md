{
  "info": {
    "name": "Aspose.Storage API Delete Storage File Path",
    "_postman_id": "bd131a95-7e98-40cd-bc62-99540d10af54",
    "description": "The resource represents customers file at server file sto",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Storage",
      "item": [
        {
          "id": "b98ef9b1-be02-40d2-9c44-c4f83990de50",
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
              "id": "43b53999-b0fd-4c34-a340-527acaa815e9"
            }
          ]
        },
        {
          "id": "68b78f51-a26d-49cc-975d-85ed97c233f9",
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
              "id": "99a1ed5f-2392-4912-b9e8-3efa2e6d1992"
            }
          ]
        },
        {
          "id": "a19c6fad-d726-437f-b03d-47a05b243ace",
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
              "id": "a342fda2-b0b9-4409-aad0-1783816e0604"
            }
          ]
        }
      ]
    }
  ]
}