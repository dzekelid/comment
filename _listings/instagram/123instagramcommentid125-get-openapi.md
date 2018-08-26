---
swagger: "2.0"
x-collection-name: Instagram
x-complete: 0
info:
  title: Instagram Instagram Comment
  version: 1.0.0
  description: Instagram Comment
host: graph.facebook.com
basePath: /v3.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /&#123;instagram-comment-id&#125;:
    get:
      summary: Instagram Comment
      description: Instagram Comment
      operationId: getInstagramComment
      x-api-path-slug: 123instagramcommentid125-get
      parameters:
      - in: query
        name: comment_typeenum
        description: Enum indicating the type of comment &#123;CAPTION, NORMAL, UNKNOWN&#125;
        type: string
      - in: query
        name: created_atdatetime
        description: Creation time of the comment in milliseconds
        type: string
      - in: query
        name: idstring
        description: Base 64 encoded string of instagram_media_id and instagram_comment_id
        type: string
      - in: query
        name: instagram_comment_idnumeric string
        description: Id of the comment in instagram
        type: string
      - in: query
        name: instagram_userInstagramUser
        description: Instagram user who made the comment
        type: string
      - in: query
        name: mentioned_instagram_userslistInstagramUser
        description: Instagram users that are mentioned in the comment
        type: string
      - in: query
        name: messagestring
        description: Textual message content of the Instagram comment
        type: string
      responses:
        200:
          description: OK
      tags:
      - Instagram
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