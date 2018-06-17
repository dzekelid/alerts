---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 0
info:
  title: ClimaCell Put Alerts Alert
  description: |-
    ### Update an Alert

    Updates the details of an Alert designated by its ```alert_id```.
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
      description: "### Create an Alert\nCreates a new Alert with the following information:\n\n*
        ```name``` - Alert Name\n* ```location_name``` - Location name for which the
        alert pertains (location has to be created earlier)\n* ```notice``` - Prior
        notice in seconds\n* ```conditions``` - logical expression defining a weather
        event such as: rain with intensity of more than 1 mm/hr. Several expressions
        can be concatenated with \u201Cor\u201D logical operator. An alert will trigger
        for it if any of its contained conditions are met. ORs can contain any number
        of conditions.\n\nNOTE:\u200B AND condition \u200B coming soon\n\n### In addition
        to the format below, this is an example with an \"OR\" conditional statement:\n
        \ ```\n  {\n    \"name\": \"alert with or\",\n    \"location_name\": \"your-location-name\",\n
        \   \"notice\": 3600,\n    \"conditions\": [\n      {\n        \"or\": [\n
        \         {\n            \"parameter\": \"Rain\",\n            \"value\":
        0.15,\n            \"operator\": \"lt\"\n          },\n          {\n            \"parameter\":
        \"Temperature\",\n            \"value\": 25,\n            \"operator\": \"lt\"\n
        \         }\n        ]\n      }\n    ],\n    \"groups\": [\n      {\n        \"name\":
        \"your-group-name\",\n        \"delivery\": {\n          \"sms\": true,\n
        \         \"email\": false\n        }\n      }\n    ],\n    \"webhooks\":
        [507f1f77bcf86cd799439011]\n  }\n  ```\n### In addition to the format below,
        this is an example with an \"AND\" conditional statement:\n\n  ```\n  {\n
        \   \"name\": \"alert with AND conditions\",\n    \"location_name\": \"your-location-name\",\n
        \   \"notice\": 3600,\n    \"conditions\": [\n      {\n        \"parameter\":
        \"Rain\",\n        \"value\": 0.15,\n        \"operator\": \"gt\"\n      },\n
        \     {\n        \"parameter\": \"Temperature\",\n        \"value\": 40,\n
        \       \"operator\": \"lt\"\n      }\n    ],\n    \"groups\": [\n      {\n
        \       \"name\": \"your-group-name\",\n        \"delivery\": {\n          \"sms\":
        true,\n          \"email\": false\n        }\n      }\n    ],\n    \"webhooks\":
        [507f1f77bcf86cd799439011]\n  }\n  ```"
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