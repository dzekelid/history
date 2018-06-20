---
swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 0
info:
  title: Jumpseller Post Orders History
  description: ""
  version: "1"
host: api.jumpseller.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /orders/{id}/history.json:
    get:
      summary: Get Orders History
      description: ""
      operationId: getOrdersHistory.json
      x-api-path-slug: ordersidhistory-json-get
      parameters:
      - in: path
        name: id
        description: Id of the Order
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Id
      - History
      - Json
    post:
      summary: Post Orders History
      description: ""
      operationId: postOrdersHistory.json
      x-api-path-slug: ordersidhistory-json-post
      parameters:
      - in: body
        name: body
        description: Order History parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: Id of the OrderHistory
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Orders
      - Id
      - History
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