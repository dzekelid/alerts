---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Sends alerts for all current platform issues.
  version: 1.0.0
  description: Sends alerts for all current platform issues..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/coreplatformstate/sendpendingalerts:
    post:
      summary: Sends alerts for all current platform issues.
      description: Sends alerts for all current platform issues..
      operationId: CorePlatformState_SendPendingAlerts
      x-api-path-slug: apicoreplatformstatesendpendingalerts-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Alerts
      - Current
      - Platform
      - Issues
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