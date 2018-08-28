---
swagger: "2.0"
x-collection-name: NPR
x-complete: 0
info:
  title: NPR Get recent ratings the logged-in user has submitted
  description: This endpoint provides the list of recently-rated audio recommendations
    that the logged-in user has consumed. Some rated recommendations are filtered,
    such as sponsorship and donation.
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listening/v2/history:
    get:
      summary: Get recent ratings the logged-in user has submitted
      description: This endpoint provides the list of recently-rated audio recommendations
        that the logged-in user has consumed. Some rated recommendations are filtered,
        such as sponsorship and donation.
      operationId: getHistory
      x-api-path-slug: listeningv2history-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - News
      - Listening
      - History
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---