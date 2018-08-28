{
  "info": {
    "name": "Plentymarkets Upload a file to the inbox",
    "_postman_id": "ab41958e-f1c6-4c4e-abb0-69a5c9f28f4d",
    "description": "Uploads a file to the inbox. The storage key (i.e. file path) must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "File",
      "item": [
        {
          "id": "6334620f-ccf2-4f66-8f4e-39e888751cfa",
          "name": "getRestStorageFrontendFile",
          "request": {
            "url": "http://example.com/rest/storage/frontend/file?key=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get file information for a single object in frontend storage. append public cloudfront url to retrieved object.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f019b4d-322e-467d-920d-502a37bd4472"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "9e50a4b6-acb5-4820-a3eb-cd53b0af3b22",
          "name": "postRestStorageFrontendFile",
          "request": {
            "url": "http://example.com/rest/storage/frontend/file?key=%7B%7D&maxAge=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "If file is an image, generate a thumbnail and store dimensions in metadata."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6413db67-3d2d-4579-b42f-7cd7ad3d8df8"
            }
          ]
        },
        {
          "id": "e6606f78-7f8e-4c1e-9515-873fe180416a",
          "name": "postRestStoragePluginsInbox",
          "request": {
            "url": "http://example.com/rest/storage/plugins/inbox?key=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Uploads a file to the inbox. The storage key (i.e. file path) must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1d8a115-3440-41e6-9f83-98a32906cc5f"
            }
          ]
        }
      ]
    },
    {
      "name": "URLa",
      "item": [
        {
          "id": "879136c4-a35c-49ff-8748-c5f5cf099528",
          "name": "getRestStorageOrderPropertiesObjectUrl",
          "request": {
            "url": "http://example.com/rest/storage/order-properties/object-url?key=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10\nminutes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "001fadc7-005a-424f-be44-8131131e830d"
            }
          ]
        }
      ]
    }
  ]
}