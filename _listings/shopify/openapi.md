---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 1
info:
  title: Shopify API
  description: todo-add-description
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/comments/2941387470.json:
    put:
      summary: Update a comment
      description: Update a comment.
      operationId: putAdminComments2941387470.json
      x-api-path-slug: admincomments2941387470-json-put
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Comment
  /admin/comments/#{id}.json:
    get:
      summary: Get a single comment
      description: Get a single comment.
      operationId: getAdminComments#.json
      x-api-path-slug: admincommentsid-json-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Single
      - Comment
  /admin/comments/2941387470/spam.json:
    post:
      summary: Mark a comment as Spam
      description: Mark a comment as spam.
      operationId: postAdminComments2941387470Spam.json
      x-api-path-slug: admincomments2941387470spam-json-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Mark
      - Comment
      - As
      - Spam
  /admin/comments/2941387470/remove.json:
    post:
      summary: Remove a comment
      description: Remove a comment.
      operationId: postAdminComments2941387470Remove.json
      x-api-path-slug: admincomments2941387470remove-json-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Remove
      - Comment
  /admin/comments/2941387470/approve.json:
    post:
      summary: Approve a comment
      description: Approve a comment.
      operationId: postAdminComments2941387470Approve.json
      x-api-path-slug: admincomments2941387470approve-json-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Approve
      - Comment
  /admin/comments/2941387470/not_spam.json:
    post:
      summary: Mark a comment as not spam
      description: Mark a comment as not spam.
      operationId: postAdminComments2941387470NotSpam.json
      x-api-path-slug: admincomments2941387470not-spam-json-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Mark
      - Comment
      - As
      - Not
      - Spam
  /admin/comments/2941387470/restore.json:
    post:
      summary: restore a comment
      description: Restore a comment.
      operationId: postAdminComments2941387470Restore.json
      x-api-path-slug: admincomments2941387470restore-json-post
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Restore
      - Comment
---