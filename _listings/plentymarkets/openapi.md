swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/listings/markets/histories:
    get:
      summary: List listing market history
      description: Lists listing market history by filter options.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistories-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing market histories
          with given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing market histories
          with a given directory ID
      - in: query
        name: duration
        description: Filter that restricts the search result to listing market histories
          with given duration
      - in: query
        name: externalId
        description: Filter that restricts the search result to listing market histories
          with given external id
      - in: query
        name: firstPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with first platform category ID equal to the given ID
      - in: query
        name: firstShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with first shop category ID equal to the given ID
      - in: query
        name: isClickAndCollect
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Click & Collect
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Plus
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing market histories
          that belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lastSale
        description: Filter that restricts the search result to listing market histories
          with last sale before given date
      - in: query
        name: listingId
        description: Filter that restricts the search result to listing market histories
          that belong to a given listing ID
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market histories
          that match the given listing market ID(s)
      - in: query
        name: listingTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing of a custom type ID
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing market histories
          with given referrer ID
      - in: query
        name: secondPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with second platform category ID equal to the given ID
      - in: query
        name: secondShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with second shop category ID equal to the given ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing market histories
          that belong to a given shipping profile
      - in: query
        name: statusId
        description: Filter that restricts the search result to listing market histories
          with a custom status status ID
      - in: query
        name: stockCondition
        description: Filter that restricts the search result to listing market histories
          with a custom stock condition
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing with a custom stock dependence type ID
      - in: query
        name: textData
        description: Filter that restricts the search result to listing market histories
          that match given text in listing title or description
      - in: query
        name: thirdShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with third shop category ID equal to the given ID
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to listing market histories
          that were last updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to listing market histories
          that were last updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to listing market histories
          that match the given variation ID(s)
      - in: query
        name: variations
        description: Filter that restricts the search result to listing market histories
          with a custom variation condition
      - in: query
        name: verified
        description: Filter that restricts the search result to listing market histories
          that are verified
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - History
  /rest/listings/markets/histories/{id}:
    get:
      summary: Get a listing market history
      description: Gets a listing market history by given ID.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistoriesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Market
      - History
  /rest/orders/{orderId}/status-history:
    get:
      summary: Get the status history of an order
      description: Gets the status of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderStatusHistory
      x-api-path-slug: restordersorderidstatushistory-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Status
      - History
      - Of
      - Order