---
swagger: "2.0"
x-collection-name: Square
x-complete: 1
info:
  title: Square Connect
  description: client-library-for-accessing-the-square-connect-apis
  termsOfService: https://connect.squareup.com/tos
  contact:
    name: Square Developer Platform
    url: https://squareup.com/developers
    email: developers@squareup.com
  version: "2.0"
host: connect.squareup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/me/timecards/{timecard_id}:
    put:
      summary: Modifies a timecard's details. This creates an API_EDIT event for the
        timecard. You can view a timecard's event history with the List Timecard Events
        endpoint.
      description: Modifies a timecard's details. This creates an API_EDIT event for
        the timecard. You can view a timecard's event history with the List Timecard
        Events endpoint.
      operationId: UpdateTimecard
      x-api-path-slug: v1metimecardstimecard-id-put
      parameters:
      - in: body
        name: body
        description: An object containing the fields to POST for the request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: timecard_id
        description: TThe ID of the timecard to modify
      responses:
        200:
          description: OK
      tags:
      - Modifies
      - Timecards
      - Details
      - ""
      - This
      - Creates
      - EDIT
      - Eventthe
      - Timecard
      - ""
      - You
      - Can
      - View
      - Timecards
      - Event
      - History
      - List
      - Timecard
      - Events
      - Endpoint
  /v1/{location_id}/orders/{order_id}:
    get:
      summary: Provides comprehensive information for a single online store order,
        including the order's history.
      description: Provides comprehensive information for a single online store order,
        including the order's history.
      operationId: RetrieveOrder
      x-api-path-slug: v1location-idordersorder-id-get
      parameters:
      - in: path
        name: location_id
        description: The ID of the orders associated location
      - in: path
        name: order_id
        description: The orders Square-issued ID
      responses:
        200:
          description: OK
      tags:
      - Provides
      - Comprehensive
      - Informationa
      - Single
      - Online
      - Store
      - Order
      - ""
      - Including
      - Orders
      - History
---