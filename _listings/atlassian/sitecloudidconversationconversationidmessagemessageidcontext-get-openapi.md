---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Software Cloud API Get conversation history contextually
  description: Authentication required, with scope participate:conversation This method
    returns messages after and/or before a given messageID including the message itself.
    Default value for 'after' and 'before' query parameters is 0. Max number of messages
    returned is 75.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/{conversationId}/message:
    get:
      summary: Get conversation history
      description: "Authentication required, with scope participate:conversation This
        method returns messages after/before a given messageIDs or/and timestamps.
        If these parameters are omitted the method returns conversation\u2019s latest
        messages. Max number of messages returned is 75."
      operationId: ConversationMessagesGetHandler
      x-api-path-slug: sitecloudidconversationconversationidmessage-get
      parameters:
      - in: query
        name: afterMessage
        description: Returns at most 75 latest messages after a provided messageID
      - in: query
        name: afterTimestamp
        description: Returns at most 75 latest messages after a provided RFC3339 timestamp
          (2006-01-02T15:04:05+07:00)
      - in: query
        name: beforeMessage
        description: Returns at most 75 messages before a provided messageID
      - in: query
        name: beforeTimestamp
        description: Returns at most 75 messages before a provided RFC3339 timestamp
          (2006-01-02T15:04:05+07:00)
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: query
        name: limit
        description: The maximum number of results
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - History
  /site/{cloudId}/conversation/{conversationId}/message/{messageId}/context:
    get:
      summary: Get conversation history contextually
      description: Authentication required, with scope participate:conversation This
        method returns messages after and/or before a given messageID including the
        message itself. Default value for 'after' and 'before' query parameters is
        0. Max number of messages returned is 75.
      operationId: ConversationContextMessagesGetHandler
      x-api-path-slug: sitecloudidconversationconversationidmessagemessageidcontext-get
      parameters:
      - in: query
        name: after
        description: A number of messages to return after the Message
      - in: query
        name: before
        description: A number of messages to return before the Message
      - in: path
        name: cloudId
        description: The id of the site (cloudId)
      - in: path
        name: conversationId
        description: The conversation id
      - in: path
        name: messageId
        description: The ID of the Message to retrieve
      responses:
        200:
          description: OK
      tags:
      - Conversation
      - History
      - Contextually
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