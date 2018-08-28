{
  "info": {
    "name": "Plentymarkets Get the URL for a order property file",
    "_postman_id": "37bed45c-1b93-4629-90fd-276b8a0feae2",
    "description": "Gets the URL of a order property file. The storage key must be specified. The returned URL expires after 10\nminutes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "File",
      "item": [
        {
          "id": "056ac4e0-8b2e-439d-8b3c-7e0773205c0a",
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
              "id": "5007480f-5c37-4519-9287-8b73b47907ed"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "617df201-a5b9-4b90-b710-212bd6861e22",
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
              "id": "9e9dbbff-ebb4-4a6d-9018-95b373f89021"
            }
          ]
        }
      ]
    },
    {
      "name": "URLa",
      "item": [
        {
          "id": "14d329a0-6426-4a4c-a997-cd627b6be946",
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
              "id": "4174541b-edfa-447c-9e3a-8f12aff8fdbc"
            }
          ]
        }
      ]
    }
  ]
}