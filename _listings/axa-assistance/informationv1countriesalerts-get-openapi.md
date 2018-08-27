---
swagger: "2.0"
x-collection-name: AXA Assistance
x-complete: 0
info:
  title: AXA Assistance Retrieve the latest alerts worldwide
  description: Retrieve the latest alerts worldwide
  version: 1.0.0
host: sandbox.api.axa-assistance.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /information/v1/countries/alerts:
    get:
      summary: Retrieve the latest alerts worldwide
      description: Retrieve the latest alerts worldwide
      operationId: getInformationV1CountriesAlerts
      x-api-path-slug: informationv1countriesalerts-get
      parameters:
      - in: header
        name: accept-language
        description: Language/Country
      responses:
        200:
          description: OK
      tags:
      - Insurance
      - Retrieve
      - the
      - latest
      - alertAssistance
      - worldwide
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