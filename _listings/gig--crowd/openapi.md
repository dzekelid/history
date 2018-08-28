swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/gigme/event/history:
    get:
      summary: Get Gigme Event History
      description: Get gigme event history.
      operationId: getApiV1GigmeEventHistory
      x-api-path-slug: apiv1gigmeeventhistory-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Gigme
      - Event
      - History
  /api/v1/request/{requestId}/history:
    get:
      summary: Get Request Requestid History
      description: Get request requestid history.
      operationId: getApiV1RequestRequestHistory
      x-api-path-slug: apiv1requestrequestidhistory-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - History