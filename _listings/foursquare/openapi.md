---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
  description: checkin-explore-your-city-and-connect-people-and-places-bapi-v2-b
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{USER_ID}/venuehistory:
    get:
      summary: Get Users Venuehistory
      description: /users/{USER_ID}/todos
      operationId: usersuser-idtodos
      x-api-path-slug: usersuser-idvenuehistory-get
      parameters:
      - in: query
        name: afterTimestamp
        description: Seconds after epoch
      - in: query
        name: beforeTimestamp
        description: Seconds since epoch
      - in: query
        name: categoryId
        description: Limits returned venues to those in this category
      - in: query
        name: USER_ID
        description: Identity of the user to get details for
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Venuehistory
---