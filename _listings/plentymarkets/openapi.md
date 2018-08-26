---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/comments:
    post:
      summary: Create a comment
      description: Creates a comment.
      operationId: postRestComments
      x-api-path-slug: restcomments-post
      parameters:
      - in: body
        name: /rest/comments
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Comment
  /rest/comments/{commentId}:
    delete:
      summary: Delete a comment
      description: Deletes a comment. The ID of the comment must be specified.
      operationId: deleteRestCommentsComment
      x-api-path-slug: restcommentscommentid-delete
      parameters:
      - in: path
        name: commentId
      responses:
        200:
          description: OK
      tags:
      - Comment
    get:
      summary: Get a comment
      description: Gets a comment. The ID of the comment must be specified.
      operationId: getRestCommentsComment
      x-api-path-slug: restcommentscommentid-get
      parameters:
      - in: path
        name: commentId
      responses:
        200:
          description: OK
      tags:
      - Comment
  /rest/feedbacks/comment:
    post:
      summary: Create a feedback comment
      description: Creates a feedback comment.
      operationId: postRestFeedbacksComment
      x-api-path-slug: restfeedbackscomment-post
      parameters:
      - in: query
        name: commentRelationTargetId
        description: The ID of the comments target
      - in: query
        name: commentRelationTargetTypeId
        description: The type ID of the comments target
      - in: query
        name: message
        description: Feedback comment message
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Comment
  /rest/feedbacks/comment/{commentId}:
    delete:
      summary: Delete a feedback comment
      description: Deletes a feedback comment. The ID of the feedback comment must
        be specified.
      operationId: deleteRestFeedbacksCommentComment
      x-api-path-slug: restfeedbackscommentcommentid-delete
      parameters:
      - in: path
        name: commentId
      - in: query
        name: feedbackCommentId
        description: The ID of the feedback comment
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Comment
    get:
      summary: Get a feedback comment
      description: Gets a feedback comment. The ID of the feedback comment must be
        specified.
      operationId: getRestFeedbacksCommentComment
      x-api-path-slug: restfeedbackscommentcommentid-get
      parameters:
      - in: path
        name: commentId
      - in: query
        name: feedbackCommentId
        description: The ID of the feedback comment
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Comment
---