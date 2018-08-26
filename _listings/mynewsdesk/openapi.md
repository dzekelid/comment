---
swagger: "2.0"
x-collection-name: Mynewsdesk
x-complete: 1
info:
  title: My News Desk Pressroom List
  description: mynewsdesk-webservice-for-newsroom-is-a-way-for-you-as-a-registered-customer-to-fetch-information-from-your-newsroom-at-mynewsdesk-to-any-system--you-can-get-all-your-information-as-xml-and-create-email-subscriptions-to-your-material-
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
---