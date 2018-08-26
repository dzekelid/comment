---
swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 0
info:
  title: My News Desk Pressroom List Create Comment
  description: Create Comment
  termsOfService: http://www.mynewsdesk.com/about/terms-and-conditions?locale=en
  version: v1
host: www.mynewsdesk.com
basePath: /services/pressroom/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  create_comment/:
    get:
      summary: Create Comment
      description: Create Comment
      operationId: getCreateComment
      x-api-path-slug: create-comment-get
      parameters:
      - in: query
        name: blog
        description: URL of commenters blog/website
      - in: query
        name: body
        description: Content of comment
      - in: query
        name: commentable_id
        description: ID of the material that is commented
      - in: query
        name: email
        description: Email address of commenter
      - in: query
        name: name
        description: Name of commenter
      - in: query
        name: type_of_media
        description: Type of material
      - in: path
        name: unique key
        description: The MyNewsDesk API Key
      - in: query
        name: user_ip
        description: IP number of commenter
      responses:
        200:
          description: OK
      tags:
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