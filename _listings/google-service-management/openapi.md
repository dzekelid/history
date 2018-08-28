---
swagger: "2.0"
x-collection-name: Google Service Management
x-complete: 1
info:
  title: Google Service Management
  description: google-service-management-allows-service-producers-to-publish-their-services-on-google-cloud-platform-so-that-they-can-be-discovered-and-used-by-service-consumers-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: servicemanagement.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/services/{serviceName}/rollouts:
    get:
      summary: Get History
      description: |-
        Lists the history of the service configuration rollouts for a managed
        service, from the newest to the oldest.
      operationId: servicemanagement.services.rollouts.list
      x-api-path-slug: v1servicesservicenamerollouts-get
      parameters:
      - in: query
        name: pageSize
        description: The max number of items to include in the response list
      - in: query
        name: pageToken
        description: The token of the page to retrieve
      - in: path
        name: serviceName
        description: The name of the service
      responses:
        200:
          description: OK
      tags:
      - Service History
---