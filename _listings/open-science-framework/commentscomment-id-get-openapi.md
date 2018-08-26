---
swagger: "2.0"
x-collection-name: Open Science Framework
x-complete: 0
info:
  title: Open Science Framework Retrieve a comment
  description: |-
    Retrieves the details of a comment
    ####Returns
    Returns a JSON object with a `data` key containing the representation of the requested comment, if the request was successful.

    If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
  contact:
    name: OSF
    url: https://osf.io/support
    email: support@osf.io
  version: "2.0"
host: test-api.osf.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /comments/{comment_id}/:
    delete:
      summary: Delete a comment
      description: |-
        Deletes a comment. This action can be undone by setting deleted to False in a comment update request.
        #### Returns
        If the request is successful, no content is returned.

        If the request is unsuccessful, a JSON object with an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: comments_delete
      x-api-path-slug: commentscomment-id-delete
      parameters:
      - in: path
        name: comment_id
        description: The unique identifier of the comment you wish to delete
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Comment
    get:
      summary: Retrieve a comment
      description: |-
        Retrieves the details of a comment
        ####Returns
        Returns a JSON object with a `data` key containing the representation of the requested comment, if the request was successful.

        If the request is unsuccessful, an `errors` key containing information about the failure will be returned. Refer to the [list of error codes](#Introduction_error_codes) to understand why this request may have failed.
      operationId: comments_read
      x-api-path-slug: commentscomment-id-get
      parameters:
      - in: path
        name: comment_id
        description: The unique identifier of the comment you wish to retrieve
      responses:
        200:
          description: OK
      tags:
      - Comments
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