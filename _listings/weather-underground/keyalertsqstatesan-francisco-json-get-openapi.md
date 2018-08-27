---
swagger: "2.0"
x-collection-name: Weather Underground
x-complete: 0
info:
  title: Weather Underground Get Key Alerts Q Ca San Francisco
  description: This example will return active severe alerts for San Francisco, California.    This
    request only works in the USA, Canada and Europe.
  version: 1.0.0
host: api.wunderground.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{key}/alerts/q/{state}/San_Francisco.json:
    get:
      summary: Get Key Alerts Q Ca San Francisco
      description: This example will return active severe alerts for San Francisco,
        California.    This request only works in the USA, Canada and Europe.
      operationId: Get_alerts_example_
      x-api-path-slug: keyalertsqstatesan-francisco-json-get
      parameters:
      - in: path
        name: city
        description: The city
        type: string
        format: string
      - in: path
        name: state
        description: The state
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Key
      - Alerts
      - Q
      - CA
      - San
      - Francisco
      - Json
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