---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/{requestId}/comments:
    get:
      summary: Get Request Requestid Comments
      description: Get request requestid comments.
      operationId: getApiV1RequestRequestComments
      x-api-path-slug: apiv1requestrequestidcomments-get
      parameters:
      - in: header
        name: Authorization
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Comments
    post:
      summary: Post Request Requestid Comments
      description: Post request requestid comments.
      operationId: postApiV1RequestRequestComments
      x-api-path-slug: apiv1requestrequestidcomments-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: model
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: requestId
        description: /
      responses:
        200:
          description: OK
      tags:
      - Request
      - Requestid
      - Comments
---