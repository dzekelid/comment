---
swagger: "2.0"
x-collection-name: Flat
x-complete: 1
info:
  title: Flat
  description: the-flat-api-allows-you-to-easily-extend-the-abilities-of-the-flat-platformhttpsflat-io-with-a-wide-range-of-use-cases-including-the-following-creating-and-importing-new-music-scores-using-musicxml-or-midi-files--browsing-updating-copying-exporting-the-users-scores-for-example-in-mp3-wav-or-midi--managing-educational-resources-with-flat-for-education-creating--updating-the-organization-accounts-the-classes-rosters-and-assignments--the-flat-api-is-built-on-http--our-api-is-restful-it-has-predictable-resource-urls--it-returns-http-response-codes-to-indicate-errors--it-also-accepts-and-returns-json-in-the-http-body--
  termsOfService: https://flat.io/legal
  contact:
    name: Flat
    url: https://flat.io/support
    email: developers@flat.io
  version: 2.1.0
host: api.flat.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /scores/{score}/comments:
    post:
      summary: Post a new comment
      description: |-
        Post a document or a contextualized comment on a document.

        Please note that this method includes an anti-spam system for public scores. We don't guarantee that your comments will be accepted and displayed to end-user. Comments are be blocked by returning a `403` HTTP error and hidden from other users when the `spam` property is `true`.
      operationId: postScoreComment
      x-api-path-slug: scoresscorecomments-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - New
      - Comment
  /scores/{score}/comments/{comment}:
    delete:
      summary: Delete a comment
      description: ""
      operationId: deleteScoreComment
      x-api-path-slug: scoresscorecommentscomment-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Comment
    put:
      summary: Update an existing comment
      description: ""
      operationId: updateScoreComment
      x-api-path-slug: scoresscorecommentscomment-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Existing
      - Comment
  /scores/{score}/comments/{comment}/resolved:
    delete:
      summary: Mark the comment as unresolved
      description: ""
      operationId: markScoreCommentUnresolved
      x-api-path-slug: scoresscorecommentscommentresolved-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Mark
      - Comment
      - As
      - Unresolved
    put:
      summary: Mark the comment as resolved
      description: ""
      operationId: markScoreCommentResolved
      x-api-path-slug: scoresscorecommentscommentresolved-put
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Mark
      - Comment
      - As
      - Resolved
---