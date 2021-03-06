---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API Get Parameter History
  version: 1.0.0
  description: Query a list of all parameters used by the AWS account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetParameterHistory:
    get:
      summary: Get Parameter History
      description: Query a list of all parameters used by the AWS account.
      operationId: getParameterHistory
      x-api-path-slug: actiongetparameterhistory-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: Name
        description: The name of a parameter you want to query
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WithDecryption
        description: Return decrypted values for secure string parameters
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter
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