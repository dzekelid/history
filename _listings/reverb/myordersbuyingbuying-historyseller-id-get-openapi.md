---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: reverb Get My Orders Buying Buying History Seller
  description: Get my orders buying buying history seller.
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/orders/selling/buyer_history/{buyer_id}:
    get:
      summary: Get My Orders Selling Buyer History Buyer
      description: Get my orders selling buyer history buyer.
      operationId: getMyOrdersSellingBuyerHistoryBuyer
      x-api-path-slug: myorderssellingbuyer-historybuyer-id-get
      parameters:
      - in: path
        name: buyer_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Selling
      - Buyer
      - History
      - Buyer
      - Id
  /my/orders/buying/buying_history/{seller_id}:
    get:
      summary: Get My Orders Buying Buying History Seller
      description: Get my orders buying buying history seller.
      operationId: getMyOrdersBuyingBuyingHistorySeller
      x-api-path-slug: myordersbuyingbuying-historyseller-id-get
      parameters:
      - in: path
        name: seller_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Orders
      - Buying
      - Buying
      - History
      - Seller
      - Id
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