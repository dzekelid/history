---
swagger: "2.0"
x-collection-name: Bitly
x-complete: 0
info:
  title: Bitly User API User Link History
  description: Returns entries from a users link history in reverse chronological
    order.
  termsOfService: http://dev.bitly.com/best_practices.html
  version: v3
host: api-ssl.bitly.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/user/link_history:
    get:
      summary: User Link History
      description: Returns entries from a users link history in reverse chronological
        order.
      operationId: userLinkHistory
      x-api-path-slug: v3userlink-history-get
      parameters:
      - in: query
        name: archived
        description: on, offor both whether to include or exclude archived history
          entries
      - in: query
        name: campaign_id
        description: filter to return only links for the given campaign_id, can be
          provided multiple times
      - in: query
        name: created_after
        description: timestamp as an integer unix epoch
      - in: query
        name: created_before
        description: timestamp as an integer unix epoch
      - in: query
        name: exact_domain
        description: n exact domain to filter on history entries
      - in: query
        name: expand_client_id
        description: whether to provide additional information about encoding application
      - in: query
        name: keyword
        description: custom keyword to filter on history entries
      - in: query
        name: limit
        description: 'integer in the range 1 to 100 default: 50, specifying the max
          number of results to return'
      - in: query
        name: link
        description: optional the Bitlink or Bitlinks to return metadata for (when
          specified, overrides all other options), can be provided multiple times
      - in: query
        name: modified_after
        description: timestamp as an integer unix epoch
      - in: query
        name: offset
        description: integer specifying the numbered result at which to start (for
          pagination)
      - in: query
        name: private
        description: on, off and both whether to include or exclude private history
          entries
      - in: query
        name: query
        description: optional ad hoc text search string
      - in: query
        name: root_domain
        description: a root domain to filter on history entries
      - in: query
        name: user
        description: the user for whom to retrieve history entries (if different from
          authenticated user)
      responses:
        200:
          description: OK
      tags:
      - User
      - Link
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