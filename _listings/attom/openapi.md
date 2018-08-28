swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /assessmenthistory/detail:
    get:
      summary: Returns assessment history and property details.
      description: Get a full detail of property characteristics and assessment history
        information for a specific property.
      operationId: assessmentHistoryDetailID
      x-api-path-slug: assessmenthistorydetail-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: id
        description: property id
      responses:
        2:
          description: Successful response
        200:
          description: OK
      tags:
      - Returns
      - Assessment
      - History
      - Property
      - Details
  /saleshistory/basichistory:
    get:
      summary: Returns basic transaction and loan history on a property.
      description: Get the basic transaction and loan history on a property for a
        specific address.
      operationId: saleHistoryBasicHistory
      x-api-path-slug: saleshistorybasichistory-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Basic
      - Transaction
      - Loan
      - History
      - "On"
      - Property
  /saleshistory/expandedhistory:
    get:
      summary: Returns detailed transaction, pre-foreclosure and loan history on a
        property.
      description: Get the detailed transaction, pre-foreclosure and loan history
        on a property for a specific address.
      operationId: saleHistoryExpandedHistory
      x-api-path-slug: saleshistoryexpandedhistory-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: query
        name: address1
        description: The first line of the mailing address
      - in: query
        name: address2
        description: The second line of the mailing address
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Detailed
      - Transaction
      - ""
      - Pre-foreclosure
      - Loan
      - History
      - "On"
      - Property