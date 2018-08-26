---
swagger: "2.0"
x-collection-name: Datadog
x-complete: 1
info:
  title: DataDog Merged API
  version: 1.0.0
basePath: api/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  comments/:comment_id:
    put:
      summary: Put Comments Comment
      description: PUT comments comment
      operationId: putCommentsComment
      x-api-path-slug: commentscomment-id-put
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Comments
      - Comment
    delete:
      summary: Delete Comments Comment
      description: DELETE comments comment
      operationId: deleteCommentsComment
      x-api-path-slug: commentscomment-id-delete
      responses:
        200:
          description: OK
      tags:
      - Monitoring
      - Comments
      - Comment
---