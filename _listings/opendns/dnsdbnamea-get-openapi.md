---
swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 0
info:
  title: OpenDNS DNS RR History
  version: 1.0.0
  description: The DNS database can be used to query the history that OpenDNS has
    seen for a given domain.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dnsdb/{name}/a/:
    get:
      summary: DNS RR History
      description: The DNS database can be used to query the history that OpenDNS
        has seen for a given domain.
      operationId: rrHistory
      x-api-path-slug: dnsdbnamea-get
      parameters:
      - in: path
        name: name
        description: Domain Name
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
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