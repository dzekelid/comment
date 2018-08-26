---
swagger: "2.0"
x-collection-name: UK National Archives
x-complete: 1
info:
  title: Getty Images
  description: build-applications-using-the-worlds-most-powerful-imagery
  version: "3.0"
host: api.gettyimages.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/boards/{board_id}/comments/{comment_id}:
    delete:
      summary: Delete Boards Board Comments Comment
      description: <b>***beta***</b> delete a comment from a board.
      operationId: deleteV3BoardsBoardCommentsComment
      x-api-path-slug: v3boardsboard-idcommentscomment-id-delete
      parameters:
      - in: header
        name: Accept-Language
        description: Provide a header to specify the language of result values
      - in: header
        name: Authorization
        description: Provide access token in the format of Bearer {token}
      - in: path
        name: board_id
        description: Specify the board containing the comment to delete
      - in: path
        name: comment_id
        description: Specify the comment to delete
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Board
      - Comments
      - Comment
---