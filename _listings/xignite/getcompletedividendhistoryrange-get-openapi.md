---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Historical Get Complete Dividend History Range
  description: Get extended dividend history range for a stock.
  version: 1.0.0
host: www.xignite.com
basePath: xHistorical.json/XigniteHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetDividendHistory:
    get:
      summary: Get Dividend History
      description: Get dividend history for a stock.
      operationId: postGetdivendhistory
      x-api-path-slug: getdividendhistory-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Dividend
      - History
  /GetDividendHistoryRange:
    get:
      summary: Get Dividend History Range
      description: Get dividend history for a stock.
      operationId: postGetdivendhistoryrange
      x-api-path-slug: getdividendhistoryrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Dividend
      - History
      - Range
  /GetExtendedDividendHistory:
    get:
      summary: Get Extended Dividend History
      description: Get extended dividend history for a stock.
      operationId: postGetextendeddivendhistory
      x-api-path-slug: getextendeddividendhistory-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Extended
      - Dividend
      - History
  /GetExtendedDividendHistoryRange:
    get:
      summary: Get Extended Dividend History Range
      description: Get extended dividend history range for a stock.
      operationId: postGetextendeddivendhistoryrange
      x-api-path-slug: getextendeddividendhistoryrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Extended
      - Dividend
      - History
      - Range
  /GetCompleteDividendHistoryRange:
    get:
      summary: Get Complete Dividend History Range
      description: Get extended dividend history range for a stock.
      operationId: postGetcompletedivendhistoryrange
      x-api-path-slug: getcompletedividendhistoryrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Complete
      - Dividend
      - History
      - Range
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