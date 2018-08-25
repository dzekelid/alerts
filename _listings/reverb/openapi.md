---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/follows/{follow_id}/alert:
    delete:
      summary: Delete My Follows Follow Alert
      description: Delete my follows follow alert.
      operationId: deleteMyFollowsFollowAlert
      x-api-path-slug: myfollowsfollow-idalert-delete
      parameters:
      - in: path
        name: follow_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Follow
      - Id
      - Alert
    post:
      summary: Post My Follows Follow Alert
      description: Post my follows follow alert.
      operationId: postMyFollowsFollowAlert
      x-api-path-slug: myfollowsfollow-idalert-post
      parameters:
      - in: path
        name: follow_id
      responses:
        200:
          description: OK
      tags:
      - My
      - Follows
      - Follow
      - Id
      - Alert
---