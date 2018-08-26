---
swagger: "2.0"
x-collection-name: Box
x-complete: 0
info:
  title: Box Get Comment
  description: Used to retrieve the message and metadata about a specific comment.
    Information about the user who created the comment is also included.
  version: 1.0.0
host: api.box.com
basePath: /2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /comments/{COMMENT_ID}:
    get:
      summary: Get Comment
      description: Used to retrieve the message and metadata about a specific comment.
        Information about the user who created the comment is also included.
      operationId: getComment
      x-api-path-slug: commentscomment-id-get
      parameters:
      - in: path
        name: COMMENT_ID
      - in: query
        name: fields
        description: Attribute(s) to include in the response
      responses:
        200:
          description: OK
      tags:
      - Documents
      - Comments
      - Comment
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