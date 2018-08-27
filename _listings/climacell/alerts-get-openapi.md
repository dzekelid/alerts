---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 0
info:
  title: ClimaCell Get Alerts
  description: |-
    ### List all Alerts

    Page through a list of all your alerts. You can specify the maximum number of results to be retuned, and from which result to start.
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
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
      description: |-
        ### List all Alerts

        Page through a list of all your alerts. You can specify the maximum number of results to be retuned, and from which result to start.
      operationId: -list-all-alertspage-through-a-list-of-all-your-alerts-you-can-specify-the-maximum-number-of-results
      x-api-path-slug: alerts-get
      parameters:
      - in: query
        name: limit
        description: The maximum number of records to load
      - in: query
        name: offset
        description: The number of records to skip
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Alerts
    post:
      summary: Post Alerts
      description: |-
        ### Create an Alert
        Creates a new Alert with the following information:

        * ```name``` - Alert Name
        * ```location_name``` - Location name for which the alert pertains (location has to be created earlier)
        * ```notice``` - Prior notice in seconds
        * ```conditions``` - logical expression defining a weather event such as: rain with intensity of more than 1 mm/hr. Several expressions can be concatenated with ???or??? logical operator. An alert will trigger for it if any of its contained conditions are met. ORs can contain any number of conditions.

        NOTE:??? AND condition ??? coming soon

        ### In addition to the format below, this is an example with an "OR" conditional statement:
          ```
          {
            "name": "alert with or",
            "location_name": "your-location-name",
            "notice": 3600,
            "conditions": [
              {
                "or": [
                  {
                    "parameter": "Rain",
                    "value": 0.15,
                    "operator": "lt"
                  },
                  {
                    "parameter": "Temperature",
                    "value": 25,
                    "operator": "lt"
                  }
                ]
              }
            ],
            "groups": [
              {
                "name": "your-group-name",
                "delivery": {
                  "sms": true,
                  "email": false
                }
              }
            ],
            "webhooks": [507f1f77bcf86cd799439011]
          }
          ```
        ### In addition to the format below, this is an example with an "AND" conditional statement:

          ```
          {
            "name": "alert with AND conditions",
            "location_name": "your-location-name",
            "notice": 3600,
            "conditions": [
              {
                "parameter": "Rain",
                "value": 0.15,
                "operator": "gt"
              },
              {
                "parameter": "Temperature",
                "value": 40,
                "operator": "lt"
              }
            ],
            "groups": [
              {
                "name": "your-group-name",
                "delivery": {
                  "sms": true,
                  "email": false
                }
              }
            ],
            "webhooks": [507f1f77bcf86cd799439011]
          }
          ```
      operationId: -create-an-alertcreates-a-new-alert-with-the-following-information-name--alert-name-location-name--l
      x-api-path-slug: alerts-post
      parameters:
      - in: body
        name: alert
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Alerts
  /alerts/{alert_id}:
    get:
      summary: Get Alerts Alert
      description: |-
        ### Retrieve an Alert

        Get a single alert with its information by specifying its ```alert_id```.
      operationId: -retrieve-an-alertget-a-single-alert-with-its-information-by-specifying-its-alert-id
      x-api-path-slug: alertsalert-id-get
      parameters:
      - in: path
        name: alert_id
        description: UUID of the Alert
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Alerts
      - Alert
    put:
      summary: Put Alerts Alert
      description: |-
        ### Update an Alert

        Updates the details of an Alert designated by its ```alert_id```.
      operationId: -update-an-alertupdates-the-details-of-an-alert-designated-by-its-alert-id
      x-api-path-slug: alertsalert-id-put
      parameters:
      - in: body
        name: alert
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: alert_id
        description: UUID of the Alert
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Alerts
      - Alert
    delete:
      summary: Delete Alerts Alert
      description: |-
        ### Delete an Alert

        Removes an alert with the ```alert_id``` from the system.
      operationId: -delete-an-alertremoves-an-alert-with-the-alert-id-from-the-system
      x-api-path-slug: alertsalert-id-delete
      parameters:
      - in: path
        name: alert_id
        description: UUID of the Alert
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Alerts
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