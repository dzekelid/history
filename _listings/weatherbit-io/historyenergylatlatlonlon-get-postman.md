{
  "info": {
    "name": "Weatherbit Get History Energy Lat & Lon",
    "_postman_id": "af60bb97-4fd2-4d41-8bc6-5a5cca29aa54",
    "description": "Returns aggregate energy specific historical weather fields, over a specified time period.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "c52a8023-5548-4360-a420-6b4cff10236a",
          "name": "returns-aggregate-energy-specific-historical-weather-fields-over-a-specified-time-period",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.weatherbit.io",
              "path": [
                "v2.0",
                "history/energy?lat=:lat&lon=:lon"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "units",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "lat",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lon",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns aggregate energy specific historical weather fields, over a specified time period"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "963e263c-3845-4c57-9dbb-da8878d3ec7f"
            }
          ]
        }
      ]
    }
  ]
}