---
swagger: "2.0"
x-collection-name: Flickr
x-complete: 0
info:
  title: Flickr Places Get Shape History
  description: Return an historical list of all the shape data generated for a Places
    or Where on Earth (WOE) ID.
  version: 1.0.0
host: api.flickr.com
basePath: /services/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/?method=flickr.places.getShapeHistory:
    get:
      summary: Places Get Shape History
      description: Return an historical list of all the shape data generated for a
        Places or Where on Earth (WOE) ID.
      operationId: getRestMethodFlickr.places.getshapehistory
      x-api-path-slug: restmethodflickr-places-getshapehistory-get
      parameters:
      - in: query
        name: api_key
        description: Your API application key
      - in: query
        name: format
        description: Response format
      - in: query
        name: place_id
        description: A Flickr Places ID
      - in: query
        name: woe_id
        description: A Where On Earth (WOE) ID
      responses:
        200:
          description: OK
      tags:
      - Places
      - GetShapeHistory
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