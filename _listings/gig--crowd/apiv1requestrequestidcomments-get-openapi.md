---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Request Requestid Comments
  version: 1.0.0
  description: Get request requestid comments.
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