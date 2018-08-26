---
swagger: "2.0"
x-collection-name: Google Drive
x-complete: 1
info:
  title: Google Drive
  description: manages-files-in-drive-including-uploading-downloading-searching-detecting-changes-and-updating-sharing-permissions-
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: v3
host: www.googleapis.com
basePath: /drive/v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /files/{fileId}/comments:
    get:
      summary: Get File Comments
      description: Lists a file's comments.
      operationId: drive.comments.list
      x-api-path-slug: filesfileidcomments-get
      parameters:
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to include deleted comments
      - in: query
        name: pageSize
        description: The maximum number of comments to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      - in: query
        name: startModifiedTime
        description: The minimum value of modifiedTime for the result comments (RFC
          3339 date-time)
      responses:
        200:
          description: OK
      tags:
      - Comment
    post:
      summary: Create File Comment
      description: Creates a new comment on a file.
      operationId: drive.comments.create
      x-api-path-slug: filesfileidcomments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: fileId
        description: The ID of the file
      responses:
        200:
          description: OK
      tags:
      - Comment
  /files/{fileId}/comments/{commentId}:
    delete:
      summary: Delete File Comment
      description: Deletes a comment.
      operationId: drive.comments.delete
      x-api-path-slug: filesfileidcommentscommentid-delete
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      responses:
        200:
          description: OK
      tags:
      - Comment
    get:
      summary: Get File Comment
      description: Gets a comment by ID.
      operationId: drive.comments.get
      x-api-path-slug: filesfileidcommentscommentid-get
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to return deleted comments
      responses:
        200:
          description: OK
      tags:
      - Comment
    patch:
      summary: Update File Comment
      description: Updates a comment with patch semantics.
      operationId: drive.comments.update
      x-api-path-slug: filesfileidcommentscommentid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      responses:
        200:
          description: OK
      tags:
      - Comment
  /files/{fileId}/comments/{commentId}/replies:
    get:
      summary: Get File Comment Replies
      description: Lists a comment's replies.
      operationId: drive.replies.list
      x-api-path-slug: filesfileidcommentscommentidreplies-get
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to include deleted replies
      - in: query
        name: pageSize
        description: The maximum number of replies to return per page
      - in: query
        name: pageToken
        description: The token for continuing a previous list request on the next
          page
      responses:
        200:
          description: OK
      tags:
      - Comment
    post:
      summary: Create File Comment Reply
      description: Creates a new reply to a comment.
      operationId: drive.replies.create
      x-api-path-slug: filesfileidcommentscommentidreplies-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      responses:
        200:
          description: OK
      tags:
      - Comment
  /files/{fileId}/comments/{commentId}/replies/{replyId}:
    delete:
      summary: Delete File Comment Reply
      description: Deletes a reply.
      operationId: drive.replies.delete
      x-api-path-slug: filesfileidcommentscommentidrepliesreplyid-delete
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: replyId
        description: The ID of the reply
      responses:
        200:
          description: OK
      tags:
      - Comment
    get:
      summary: Get File Comment Reply
      description: Gets a reply by ID.
      operationId: drive.replies.get
      x-api-path-slug: filesfileidcommentscommentidrepliesreplyid-get
      parameters:
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: query
        name: includeDeleted
        description: Whether to return deleted replies
      - in: path
        name: replyId
        description: The ID of the reply
      responses:
        200:
          description: OK
      tags:
      - Comment
    patch:
      summary: Update File Comment Reply
      description: Updates a reply with patch semantics.
      operationId: drive.replies.update
      x-api-path-slug: filesfileidcommentscommentidrepliesreplyid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: commentId
        description: The ID of the comment
      - in: path
        name: fileId
        description: The ID of the file
      - in: path
        name: replyId
        description: The ID of the reply
      responses:
        200:
          description: OK
      tags:
      - Comment
---