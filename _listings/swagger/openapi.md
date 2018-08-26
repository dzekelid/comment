---
swagger: "2.0"
x-collection-name: Swagger
x-complete: 1
info:
  title: Swagger Hub Registry
  description: the-registry-api-for-swaggerhub
  contact:
    name: SwaggerHub
    url: http://swaggerhub.com
    email: info@swaggerhub.com
  version: 1.0.45
host: api.swaggerhub.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /apis/{owner}/{api}/{version}/.comment:
    get:
      summary: Returns the list of comments for the specified API
      description: Returns the list of comments for the specified api.
      operationId: getApiComments
      x-api-path-slug: apisownerapiversion-comment-get
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
    post:
      summary: Adds a new comment to the specified API
      description: Adds a new comment to the specified api.
      operationId: addApiComment
      x-api-path-slug: apisownerapiversion-comment-post
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
  /apis/{owner}/{api}/{version}/.comment/batch:
    post:
      summary: Updates passed batch of comments
      description: Updates passed batch of comments.
      operationId: updateApiComments
      x-api-path-slug: apisownerapiversion-commentbatch-post
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
      - Batch
  /apis/{owner}/{api}/{version}/.comment/{comment}:
    delete:
      summary: Deletes specified comment
      description: Deletes specified comment.
      operationId: deleteApiComment
      x-api-path-slug: apisownerapiversion-commentcomment-delete
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
      - Comment
    patch:
      summary: Updates specified comment
      description: Updates specified comment.
      operationId: updateApiComment
      x-api-path-slug: apisownerapiversion-commentcomment-patch
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
      - Comment
  /apis/{owner}/{api}/{version}/.comment/{comment}/reply:
    post:
      summary: Adds a new reply to the specified comment
      description: Adds a new reply to the specified comment.
      operationId: addApiCommentReply
      x-api-path-slug: apisownerapiversion-commentcommentreply-post
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
      - Comment
      - Reply
  /apis/{owner}/{api}/{version}/.comment/{comment}/reply/{reply}:
    delete:
      summary: Deletes specified comment reply
      description: Deletes specified comment reply.
      operationId: deleteApiCommentReply
      x-api-path-slug: apisownerapiversion-commentcommentreplyreply-delete
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: reply
        description: reply identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
      - Comment
      - Reply
      - Reply
    patch:
      summary: Updates specified comment reply
      description: Updates specified comment reply.
      operationId: updateApiCommentReply
      x-api-path-slug: apisownerapiversion-commentcommentreplyreply-patch
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: reply
        description: reply identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
      - Comment
      - Reply
      - Reply
  /apis/{owner}/{api}/{version}/.comment/{comment}/status/{status}:
    put:
      summary: Updates status to the specified comment
      description: Updates status to the specified comment.
      operationId: setApiCommentStatus
      x-api-path-slug: apisownerapiversion-commentcommentstatusstatus-put
      parameters:
      - in: path
        name: api
        description: API identifier
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: status
        description: comment status
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - APIs
      - Owner
      - Version
      - ""
      - Comment
      - Comment
      - Status
      - Status
  /domains/{owner}/{domain}/{version}/.comment:
    get:
      summary: Returns the list of comments for the specified domain
      description: Returns the list of comments for the specified domain.
      operationId: getDomainComments
      x-api-path-slug: domainsownerdomainversion-comment-get
      parameters:
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
    post:
      summary: Adds a new comment to the specified domain
      description: Adds a new comment to the specified domain.
      operationId: addDomainComment
      x-api-path-slug: domainsownerdomainversion-comment-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
  /domains/{owner}/{domain}/{version}/.comment/batch:
    post:
      summary: Updates passed batch of comments
      description: Updates passed batch of comments.
      operationId: updateDomainComments
      x-api-path-slug: domainsownerdomainversion-commentbatch-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Batch
  /domains/{owner}/{domain}/{version}/.comment/{comment}:
    delete:
      summary: Deletes specified comment
      description: Deletes specified comment.
      operationId: deleteDomainComment
      x-api-path-slug: domainsownerdomainversion-commentcomment-delete
      parameters:
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
    patch:
      summary: Updates specified comment
      description: Updates specified comment.
      operationId: updateDomainComment
      x-api-path-slug: domainsownerdomainversion-commentcomment-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
  /domains/{owner}/{domain}/{version}/.comment/{comment}/reply:
    post:
      summary: Adds a new reply to the specified comment
      description: Adds a new reply to the specified comment.
      operationId: addDomainCommentReply
      x-api-path-slug: domainsownerdomainversion-commentcommentreply-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
      - Reply
  /domains/{owner}/{domain}/{version}/.comment/{comment}/reply/{reply}:
    delete:
      summary: Deletes specified comment reply
      description: Deletes specified comment reply.
      operationId: deleteDomainCommentReply
      x-api-path-slug: domainsownerdomainversion-commentcommentreplyreply-delete
      parameters:
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: reply
        description: reply identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
      - Reply
      - Reply
    patch:
      summary: Updates specified comment reply
      description: Updates specified comment reply.
      operationId: updateDomainCommentReply
      x-api-path-slug: domainsownerdomainversion-commentcommentreplyreply-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: reply
        description: reply identifier
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
      - Reply
      - Reply
  /domains/{owner}/{domain}/{version}/.comment/{comment}/status/{status}:
    put:
      summary: Updates status to the specified comment
      description: Updates status to the specified comment.
      operationId: setDomainCommentStatus
      x-api-path-slug: domainsownerdomainversion-commentcommentstatusstatus-put
      parameters:
      - in: path
        name: comment
        description: comment identifier
      - in: path
        name: domain
        description: domain identifier
      - in: path
        name: owner
        description: API owner identifier
      - in: path
        name: status
        description: comment status
      - in: path
        name: version
        description: version identifier
      responses:
        200:
          description: OK
      tags:
      - Domains
      - Owner
      - Domain
      - Version
      - ""
      - Comment
      - Comment
      - Status
      - Status
---