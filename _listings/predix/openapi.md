swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/scheduler/jobs/{id}/history:
    get:
      summary: Retrieve job execution history of the given job.
      description: Retrieve job execution history
      operationId: retrieveJobHistory
      x-api-path-slug: apiv1schedulerjobsidhistory-get
      parameters:
      - in: header
        name: Authorization
        description: Authorization
      - in: query
        name: endTime
        description: End time in millis
      - in: path
        name: id
        description: Job id
      - in: header
        name: Predix-Zone-Id
        description: Predix-Zone-Id
      - in: query
        name: startTime
        description: Start time in millis
      responses:
        2:
          description: Successful response
        200:
          description: Successful response
      tags:
      - Retrieve
      - Job
      - Execution
      - History
      - Of
      - Given
      - Job