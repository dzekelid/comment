---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Delete comment
  description: Deletes an existing comment .
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/comment/{commentId}/properties:
    get:
      summary: Get comment property keys
      description: Returns the keys of all properties for the comment identified by
        the key or by the id.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.getCommentPropertyKeys_get
      x-api-path-slug: api2commentcommentidproperties-get
      parameters:
      - in: path
        name: commentId
        description: the comment from which keys will be returned
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
      - Keys
  /api/2/comment/{commentId}/properties/{propertyKey}:
    get:
      summary: Get comment property
      description: Returns the value of the property with a given key from the comment
        identified by the key or by the id. The user who retrieves the property is
        required to have permissions to read the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.getCommentProperty_get
      x-api-path-slug: api2commentcommentidpropertiespropertykey-get
      parameters:
      - in: path
        name: commentId
        description: the comment from which the property will be returned
      - in: path
        name: propertyKey
        description: the key of the property to return
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
    put:
      summary: Set comment property
      description: |-
        Sets the value of the specified comment's property.

        You can use this resource to store a custom data against the comment identified by the key or by the id. The user who stores the data is required to have permissions to administer the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.setCommentProperty_put
      x-api-path-slug: api2commentcommentidpropertiespropertykey-put
      parameters:
      - in: path
        name: commentId
        description: the comment on which the property will be set
      - in: path
        name: propertyKey
        description: the key of the comments property
      responses:
        200:
          description: OK
      tags:
      - Set
      - Comment
      - Property
    delete:
      summary: Delete comment property
      description: Removes the property from the comment identified by the key or
        by the id. Ths user removing the property is required to have permissions
        to administer the comment.
      operationId: com.atlassian.jira.rest.v2.issue.CommentPropertyResource.deleteCommentProperty_delete
      x-api-path-slug: api2commentcommentidpropertiespropertykey-delete
      parameters:
      - in: path
        name: commentId
        description: the comment from which the property will be removed
      - in: path
        name: propertyKey
        description: the key of the property to remove
      responses:
        200:
          description: OK
      tags:
      - Comment
      - Property
  /api/2/issue/{issueIdOrKey}/comment:
    post:
      summary: Add comment
      description: Adds a new comment to an issue.
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentResource.addComment_post
      x-api-path-slug: api2issueissueidorkeycomment-post
      parameters:
      - in: query
        name: expand
        description: 'optional flags: renderedBody (provides body rendered in HTML)'
      - in: path
        name: issueIdOrKey
        description: a string containing the issue id or key the comment will be added
          to
      responses:
        200:
          description: OK
      tags:
      - Comment
  /api/2/issue/{issueIdOrKey}/comment/{id}:
    get:
      summary: Get comment
      description: Returns a single comment.
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentResource.getComment_get
      x-api-path-slug: api2issueissueidorkeycommentid-get
      parameters:
      - in: query
        name: expand
        description: 'optional flags: renderedBody (provides body rendered in HTML)'
      - in: path
        name: id
        description: the ID of the comment to request
      - in: path
        name: issueIdOrKey
        description: of the issue the comment belongs to
      responses:
        200:
          description: OK
      tags:
      - Comment
    put:
      summary: Update comment
      description: Updates an existing comment using its JSON representation.
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentResource.updateComment_put
      x-api-path-slug: api2issueissueidorkeycommentid-put
      parameters:
      - in: query
        name: expand
        description: 'optional flags: renderedBody (provides body rendered in HTML)'
      - in: path
        name: id
        description: id of the comment to be updated
      - in: path
        name: issueIdOrKey
        description: a string containing the issue id or key the comment belongs to
      responses:
        200:
          description: OK
      tags:
      - Comment
    delete:
      summary: Delete comment
      description: Deletes an existing comment .
      operationId: com.atlassian.jira.rest.v2.issue.IssueCommentResource.deleteComment_delete
      x-api-path-slug: api2issueissueidorkeycommentid-delete
      parameters:
      - in: path
        name: id
        description: id of the comment to be deleted
      - in: path
        name: issueIdOrKey
        description: a string containing the issue id or key the comment belongs to
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