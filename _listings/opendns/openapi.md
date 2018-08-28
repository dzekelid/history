swagger: "2.0"
x-collection-name: OpenDNS
x-complete: 1
info:
  title: OpenDNS
  version: 1.0.0
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