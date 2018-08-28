swagger: "2.0"
x-collection-name: Jumpseller
x-complete: 1
info:
  title: Jumpseller
  description: explore-all-our-endpoints-with-your-own-set-of-of-access-tokens--all-changes-affect-your-production-jumpseller-store-
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