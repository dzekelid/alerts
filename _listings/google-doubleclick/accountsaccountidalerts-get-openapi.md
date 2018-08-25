---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get Alerts
  version: 1.0.0
  description: List the alerts for this Ad Exchange account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/alerts:
    get:
      summary: Get Alerts
      description: List the alerts for this Ad Exchange account.
      operationId: adexchangeseller.accounts.alerts.list
      x-api-path-slug: accountsaccountidalerts-get
      parameters:
      - in: path
        name: accountId
        description: Account owning the alerts
      - in: query
        name: locale
        description: The locale to use for translating alert messages
      responses:
        200:
          description: OK
      tags:
      - Advertising
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