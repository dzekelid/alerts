---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 0
info:
  title: Reverb Post My Follows Follow Alert
  description: Post my follows follow alert.
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