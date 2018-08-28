swagger: "2.0"
x-collection-name: Mailjet
x-complete: 1
info:
  title: Mailjet Messages API
  description: allows-you-to-list-and-view-the-details-of-a-message-an-email-processed-by-mailjet
  version: v3
host: api.mailjet.com
basePath: v3/REST/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  messagehistory/:
    get:
      summary: Message History
      description: List message history resources
      operationId: getMessagehistory
      x-api-path-slug: messagehistory-get
      parameters:
      - in: path
        name: Message
        description: ID of message for which to show the history
      responses:
        200:
          description: OK
      tags:
      - Message
      - History
  messagehistory/{id}:
    get:
      summary: Message History
      description: Get the history of a message.
      operationId: getMessagehistory
      x-api-path-slug: messagehistoryid-get
      parameters:
      - in: path
        name: id
        description: ID of the message history
      responses:
        200:
          description: OK
      tags:
      - Message
      - History