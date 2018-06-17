---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Alerts
  description: "**This endpoint allows you to retieve all of your alerts.**\n\nAlerts
    allow you to specify an email address to receive notifications regarding your
    email usage or statistics. \n* Usage alerts allow you to set the threshold at
    which an alert will be sent.\n* Stats notifications allow you to set how frequently
    you would like to receive email statistics reports. For example, \"daily\", \"weekly\",
    or \"monthly\".\n\nFor more information about alerts, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /alerts:
    get:
      summary: Get Alerts
      description: "**This endpoint allows you to retieve all of your alerts.**\n\nAlerts
        allow you to specify an email address to receive notifications regarding your
        email usage or statistics. \n* Usage alerts allow you to set the threshold
        at which an alert will be sent.\n* Stats notifications allow you to set how
        frequently you would like to receive email statistics reports. For example,
        \"daily\", \"weekly\", or \"monthly\".\n\nFor more information about alerts,
        please see our [User Guide](https://sendgrid.com/docs/User_Guide/Settings/alerts.html)."
      operationId: GET_alerts
      x-api-path-slug: alerts-get
      parameters:
      - in: header
        name: Authorization
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
      - Email
      - Alerts
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---