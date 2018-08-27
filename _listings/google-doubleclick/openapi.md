swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 1
info:
  title: Google Doubleclick Merged API
  version: 1.0.0
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