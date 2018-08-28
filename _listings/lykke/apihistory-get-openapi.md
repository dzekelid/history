---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Get API History
  version: 1.0.0
  description: Get api history.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Ethereum/history/{address}:
    get:
      summary: Get API Ethereum History Address
      description: Get api ethereum history address.
      operationId: ApiEthereumHistoryByAddressGet
      x-api-path-slug: apiethereumhistoryaddress-get
      parameters:
      - in: path
        name: address
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      - in: query
        name: count
      - in: query
        name: start
      responses:
        200:
          description: OK
      tags:
      - Ethereum
      - History
      - Ress
  /api/History:
    get:
      summary: Get API History
      description: Get api history.
      operationId: ApiHistoryGet
      x-api-path-slug: apihistory-get
      parameters:
      - in: query
        name: assetId
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - History
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