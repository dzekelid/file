{
  "info": {
    "name": "Plentymarkets Upload a single file to frontend storage.",
    "_postman_id": "7f49ede2-8521-4ffc-96b7-1d5a1abdd54b",
    "description": "If file is an image, generate a thumbnail and store dimensions in metadata.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "File",
      "item": [
        {
          "id": "f1437841-1948-4cdc-a10d-e1d1bdf0ff99",
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
              "id": "519530ee-266f-4fea-8a5d-c94d16e8d9ea"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload",
      "item": [
        {
          "id": "4f5f20fd-26db-402c-a0eb-8d907ae8305a",
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
              "id": "fffd7957-1f6d-492c-8b56-6a4d120cd2a1"
            }
          ]
        }
      ]
    }
  ]
}