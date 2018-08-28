swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
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