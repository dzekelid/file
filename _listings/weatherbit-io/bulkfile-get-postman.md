{
  "info": {
    "name": "Weatherbit Get Bulk File",
    "_postman_id": "6d859362-25cd-42a0-b61f-7c75a1236cf8",
    "description": "**(Advanced/Advanced+/Enterprise plans only)** Downloads bulk data files - OPTIONS: (forecast16d.json.gz - 16 day forecasts for cities > 1000 population, current.json.gz - Current observations for cities > 1000 population).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "3dfafdb5-d9cd-48dd-9766-060c67ce9794",
          "name": "advancedadvancedenterprise-plans-only-downloads-bulk-data-files--options-forecast16djsongz--16-day-f",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.weatherbit.io",
              "path": [
                "v2.0",
                "bulk/:file"
              ],
              "query": [
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "file",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**(Advanced/Advanced+/Enterprise plans only)** Downloads bulk data files - OPTIONS: (forecast16d"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef5660a2-bd1a-4dda-b41e-75418dd8a9f3"
            }
          ]
        }
      ]
    }
  ]
}