---
swagger: "2.0"
x-collection-name: Weather Underground
x-complete: 0
info:
  title: Weather Underground Get Key History 20101018 Q Pws Kcasanfr14
  description: This example will return historical data for a Personal Weather Station
    for the specified date.    The feature only works with JSON.    XML will come
    out soon.
  version: 1.0.0
host: api.wunderground.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{key}/history_20101018/q/SFO.json:
    get:
      summary: Get Key History 20101018 Q Sfo
      description: This example will return historical data for San Francisco, California
        for the specified date.    If you search by zip or lat/long you will get nearest
        airport.
      operationId: Get_History_example_
      x-api-path-slug: keyhistory-20101018qsfo-json-get
      parameters:
      - in: path
        name: airport_code
        description: The airport code
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Key
      - History
      - "20101018"
      - Q
      - SFO
      - Json
  /{key}/history_20101018/q/pws:KCASANFR14.json:
    get:
      summary: Get Key History 20101018 Q Pws Kcasanfr14
      description: This example will return historical data for a Personal Weather
        Station for the specified date.    The feature only works with JSON.    XML
        will come out soon.
      operationId: Get_History_example_pws_
      x-api-path-slug: keyhistory-20101018qpwskcasanfr14-json-get
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Key
      - History
      - "20101018"
      - Q
      - Pws:KCASANFR14
      - Json
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---