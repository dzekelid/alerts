swagger: "2.0"
x-collection-name: VMWare
x-complete: 1
info:
  title: vRealize Operations 6
  description: todo-add-description
  version: 1.0.0
host: example.com
basePath: /suite-api/api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/alerts/query:
    post:
      summary: Query Alerts
      description: 'TODO: Add Description'
      operationId: ApiAlertsQueryPost
      x-api-path-slug: apialertsquery-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Query
  /api/alerts/7c2a4f9a-fd04-4300-b85c-cda555782e86:
    get:
      summary: Get Alert
      description: 'TODO: Add Description'
      operationId: ApiAlerts7c2a4f9aFd044300B85cCda555782e86Get
      x-api-path-slug: apialerts7c2a4f9afd044300b85ccda555782e86-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /alerts/contributingsymptoms:
    get:
      summary: Get Alert Contributing Symptoms
      description: Added in vROps 6.7
      operationId: AlertsContributingsymptomsGet
      x-api-path-slug: alertscontributingsymptoms-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Alerts
      - Contributingsymptoms
  /api/alertdefinitions/{alertDefinitionId}:
    get:
      summary: Get Alert Definition
      description: 'TODO: Add Description'
      operationId: ApiAlertdefinitionsByAlertDefinitionIdGet
      x-api-path-slug: apialertdefinitionsalertdefinitionid-get
      parameters:
      - in: header
        name: Accept
      - in: path
        name: alertDefinitionId
      responses:
        200:
          description: OK
      tags:
      - Alertdefinitions
      - AlertDefinitionId