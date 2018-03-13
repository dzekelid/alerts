---
swagger: "2.0"
info:
  title: Alerts API
  description: The Alerts API.
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/alerts/recipients/{recipient_id} ':
    get:
      summary: Alerts Recipients {recipient_id}
      description: "\r\n\t\t\t\tGets a information about alert recipient's targets"
      operationId: -alerts-recipients-recipient-id-
      responses:
        200:
          description: OK
      tags:
      - alerts
definitions: []
x-collection-name: Pingometer
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