{
  "info": {
    "name": "Ge.tt  REST API Files Create",
    "_postman_id": "32d30116-15c4-493a-9786-408f66f3fe97",
    "description": "To upload files to Ge.tt you must first create the file under a given share. You do that by posting the filename:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Files",
      "item": [
        {
          "id": "89d6c03f-a4b6-481c-8a81-d99fea7e27dd",
          "name": "post1FilesSharenameCreate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/create"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "To upload files to Ge.tt you must first create the file under a given share. You do that by posting the filename:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c50b95b9-d9d8-496c-8900-beaa470b76bb"
            }
          ]
        }
      ]
    }
  ]
}