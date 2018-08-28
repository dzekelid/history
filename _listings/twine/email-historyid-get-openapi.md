---
swagger: "2.0"
x-collection-name: Twine
x-complete: 0
info:
  title: Twine Get an email history
  description: Get an email history by id
  version: 7.18.0
host: api.twinehealth.com
basePath: /pub
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /email_history/{id}:
    get:
      summary: Get an email history
      description: Get an email history by id
      operationId: fetchEmailHistory
      x-api-path-slug: email-historyid-get
      parameters:
      - in: path
        name: id
        description: Email history identifier
      responses:
        200:
          description: OK
      tags:
      - Wearables
      - Email
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