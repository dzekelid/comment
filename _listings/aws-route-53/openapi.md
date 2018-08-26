---
swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 1
info:
  title: AWS Route 53 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/hostedzone/Id:
    post:
      summary: Update Hosted Zone Comment
      description: Updates the hosted zone comment. Send a POST request to the/2013-04-01/hostedzone/hosted
        zone ID             resource.
      operationId: updatehostedzonecomment
      x-api-path-slug: 20130401hostedzoneid-post
      parameters:
      - in: body
        name: Comment
        description: The new comment for the hosted zone
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: Id
        description: The ID for the hosted zone for which you want to update the comment
        type: string
      - in: body
        name: UpdateHostedZoneCommentRequest
        description: Root level tag for the UpdateHostedZoneCommentRequest parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Hosted Zones
  /2013-04-01/trafficpolicy/Id/Version:
    post:
      summary: Update Traffic Policy Comment
      description: Updates the comment for a specified traffic policy version.Send
        a POST request to the /2013-04-01/trafficpolicy/ resource.The request body
        must include a document with anUpdateTrafficPolicyCommentRequest element.
      operationId: updatetrafficpolicycomment
      x-api-path-slug: 20130401trafficpolicyidversion-post
      parameters:
      - in: body
        name: Comment
        description: The new comment for the specified traffic policy and version
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: Id
        description: The value of Id for the traffic policy for which you want to
          update thecomment
        type: string
      - in: body
        name: UpdateTrafficPolicyCommentRequest
        description: Root level tag for the UpdateTrafficPolicyCommentRequest parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Traffic Policies
---