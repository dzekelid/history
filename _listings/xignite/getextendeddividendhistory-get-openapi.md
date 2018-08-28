---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Historical Get Extended Dividend History
  description: Get extended dividend history for a stock.
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
  /GetSplitHistory:
    get:
      summary: Get Split History
      description: Get split history for a stock for a date range.
      operationId: postGetsplithistory
      x-api-path-slug: getsplithistory-get
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
      - Split
      - History
  /GetCashDividendHistory:
    get:
      summary: Get Cash Dividend History
      description: Get cash dividend history for a stock for a date range.
      operationId: postGetcashdivendhistory
      x-api-path-slug: getcashdividendhistory-get
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
      - Cash
      - Dividend
      - History
  /GetCorporateActionHistory:
    get:
      summary: Get Corporate Action History
      description: Get the corporate action history for a stock for a date range.
      operationId: postGetcorporateactionhistory
      x-api-path-slug: getcorporateactionhistory-get
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
      - Corporate
      - Action
      - History
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