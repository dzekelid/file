{
  "info": {
    "name": "Kentico Cloud Upload a binary file",
    "_postman_id": "bec9535d-83d7-499b-aca7-28484c4692b4",
    "description": "Add a new file. The uploaded file will not be visible in the Kentico Cloud UI unless there is an asset using it, see how to [add an asset](https://developer.kenticocloud.com/v1/reference#content-management-api-add-asset).\r\n\r\n**Note:** Maximum size limit for binary files is 100 MB.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Upload",
      "item": [
        {
          "id": "52cd8ffb-d505-47a5-9ebf-b8044ce47f1c",
          "name": "FilesWhichBrewingFitsYou1080pxJpgPost",
          "request": {
            "url": "http://deliver.kenticocloud.com/files/which-brewing-fits-you-1080px.jpg",
            "method": "POST",
            "header": [
              {
                "key": "Content-Length",
                "value": "{}",
                "description": "Specifies the size of the binary file in bytes",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Specifies the media type of the binary data",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "File",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Add a new file. The uploaded file will not be visible in the Kentico Cloud UI unless there is an asset using it, see how to [add an asset](https://developer.kenticocloud.com/v1/reference#content-management-api-add-asset).\r\n\r\n**Note:** Maximum size limit for binary files is 100 MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8d7bf85-d290-44c5-8864-aa2274ba1639"
            }
          ]
        }
      ]
    }
  ]
}