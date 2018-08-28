---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Analytics Runtime Retrieve job execution history of the given job.
  version: 1.0.0
  description: Retrieve job execution history
host: predix-acs.run.aws-usw02-pr.ice.predix.io
basePath: /
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