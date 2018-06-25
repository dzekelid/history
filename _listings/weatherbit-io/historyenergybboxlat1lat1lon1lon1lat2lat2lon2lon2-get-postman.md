{
  "info": {
    "name": "Weatherbit Get History Energy Bbox Lat1 Lat1 &lon1 Lon1 &lat2 Lat2 &lon2 Lon2",
    "_postman_id": "e082b7e3-0e65-4b0b-8110-1d89a376221c",
    "description": "Returns aggregate energy specific historical weather fields, over a specified time period. Supply a bounding box ex: lat1=40&lon1=-78&lat2=38&lon2=-80. This API will return UP TO 150 stations, aggregated by the specified time period start_date to end_date.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "6f73932c-eebb-4023-afed-dba7c9bad649",
          "name": "returns-aggregate-energy-specific-historical-weather-fields-over-a-specified-time-period-supply-a-bo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.weatherbit.io",
              "path": [
                "v2.0",
                "history/energy/bbox?lat1=:lat1&lon1=:lon1&lat2=:lat2&lon2=:lon2"
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
                  "id": "lat1",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lat2",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lon1",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lon2",
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
              "id": "5b46ecf2-4a1d-4a57-8074-4b7c3a07cb3e"
            }
          ]
        }
      ]
    }
  ]
}