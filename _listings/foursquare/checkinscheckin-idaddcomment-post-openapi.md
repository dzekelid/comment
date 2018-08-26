---
swagger: "2.0"
x-collection-name: Foursquare
x-complete: 0
info:
  title: Foursquare Post Checkins Checkin Addcomment
  description: /checkins/recent
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /checkins/{CHECKIN_ID}/addcomment:
    post:
      summary: Post Checkins Checkin Addcomment
      description: /checkins/recent
      operationId: checkinsrecent
      x-api-path-slug: checkinscheckin-idaddcomment-post
      parameters:
      - in: query
        name: CHECKIN_ID
        description: The ID of the checkin to add a comment to
      - in: path
        name: CHECKIN_ID
      - in: query
        name: text
        description: The text of the comment, up to 200 characters
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Checkins
      - Checkin
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