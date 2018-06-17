---
swagger: "2.0"
x-collection-name: Azure Monitor
x-complete: 0
info:
  title: Azure Activity Log API Activity Log Alerts Create Or Update
  version: 2017-03-01-preview
  description: Create a new activity log alert or update an existing one.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/activityLogAlerts/{activityLogAlertName}
  : put:
      summary: Activity Log Alerts Create Or Update
      description: Create a new activity log alert or update an existing one.
      operationId: ActivityLogAlerts_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalertsactivitylogalertname-put
      parameters:
      - in: body
        name: activityLogAlert
        description: The activity log alert to create or use for the update
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Activity Log Alerts
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