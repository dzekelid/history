---
swagger: "2.0"
x-collection-name: Firebase
x-complete: 0
info:
  title: Firebase Get Executions
  description: |-
    Lists Histories for a given Project.

    The executions are sorted by creation_time in descending order. The execution_id key will be used to order the executions with the same creation_time.

    May return any of the following canonical error codes:

    - PERMISSION_DENIED - if the user is not authorized to read project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the containing History does not exist
  version: 1.0.0
host: '{project_id].firebaseio.co}'
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{projectId}/histories:
    get:
      summary: List HIstories
      description: |-
        Lists Histories for a given Project.

        The histories are sorted by modification time in descending order. The history_id key will be used to order the history with the same modification time.

        May return any of the following canonical error codes:

        - PERMISSION_DENIED - if the user is not authorized to read project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the History does not exist
      operationId: toolresults.projects.histories.list
      x-api-path-slug: projectidhistories-get
      parameters:
      - in: query
        name: filterByName
        description: If set, only return histories with the given name
      - in: query
        name: pageSize
        description: The maximum number of Histories to fetch
      - in: query
        name: pageToken
        description: A continuation token to resume the query at the next item
      - in: path
        name: projectId
        description: A Project id
      responses:
        200:
          description: OK
      tags:
      - History
    post:
      summary: Create History
      description: |-
        Creates a History.

        The returned History will have the id set.

        May return any of the following canonical error codes:

        - PERMISSION_DENIED - if the user is not authorized to write to project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the containing project does not exist
      operationId: toolresults.projects.histories.create
      x-api-path-slug: projectidhistories-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: projectId
        description: A Project id
      - in: query
        name: requestId
        description: A unique request ID for server to detect duplicated requests
      responses:
        200:
          description: OK
      tags:
      - History
  /{projectId}/histories/{historyId}:
    get:
      summary: Get History
      description: |-
        Gets a History.

        May return any of the following canonical error codes:

        - PERMISSION_DENIED - if the user is not authorized to read project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the History does not exist
      operationId: toolresults.projects.histories.get
      x-api-path-slug: projectidhistorieshistoryid-get
      parameters:
      - in: path
        name: historyId
        description: A History id
      - in: path
        name: projectId
        description: A Project id
      responses:
        200:
          description: OK
      tags:
      - History
  /{projectId}/histories/{historyId}/executions:
    get:
      summary: Get Executions
      description: |-
        Lists Histories for a given Project.

        The executions are sorted by creation_time in descending order. The execution_id key will be used to order the executions with the same creation_time.

        May return any of the following canonical error codes:

        - PERMISSION_DENIED - if the user is not authorized to read project - INVALID_ARGUMENT - if the request is malformed - NOT_FOUND - if the containing History does not exist
      operationId: toolresults.projects.histories.executions.list
      x-api-path-slug: projectidhistorieshistoryidexecutions-get
      parameters:
      - in: path
        name: historyId
        description: A History id
      - in: query
        name: pageSize
        description: The maximum number of Executions to fetch
      - in: query
        name: pageToken
        description: A continuation token to resume the query at the next item
      - in: path
        name: projectId
        description: A Project id
      responses:
        200:
          description: OK
      tags:
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