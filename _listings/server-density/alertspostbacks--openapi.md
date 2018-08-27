---
swagger: "2.0"
x-collection-name: Server Density
x-complete: 0
info:
  title: Postbacks API Creating a postback
  description: You can use this method to post data back to Server Density without
    using the agent, for example using your own scripts or to integrate in something
    custom you are doing. You will still be restricted to posting back once per minute
    using this method, as you would be using the agent.
  version: 1.0.0
host: api.serverdensity.io.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? '/alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id} '
  : ' get ':
      summary: Alerts
      description: Gets alerts filtered by set of optional parameters.
      operationId: -alertscheck-idcheck-idampseverityseverityampenabledenabledamptarget-typetarget-typeamptarget-idtarg
      x-api-path-slug: alertscheck-idcheck-idampseverityseverityampenabledenabledamptarget-typetarget-typeamptarget-idtarget-id-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/{alert_id} ':
    ' get ':
      summary: Alerts
      description: Gets alert by Id.
      operationId: -alerts-alert-id-
      x-api-path-slug: alertsalert-id-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
    ' put ':
      summary: Alerts
      description: Updates alert.
      operationId: -alerts-alert-id-
      x-api-path-slug: alertsalert-id-put
      responses:
        200:
          description: OK
      tags:
      - Alerts
    ' delete ':
      summary: Alerts
      description: Deletes alert by Id.
      operationId: -alerts-alert-id-
      x-api-path-slug: alertsalert-id-delete
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/{alert_type} ':
    ' post ':
      summary: Alerts
      description: Creates a new alert.
      operationId: -alerts-alert-type-
      x-api-path-slug: alertsalert-type-post
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipients ':
    ' get ':
      summary: Alerts Recipients
      description: Gets a list of all alert recipient's targets that are visible to
        you as a customer.
      operationId: -alerts-recipients-
      x-api-path-slug: alertsrecipients-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipients/{recipient_id} ':
    ' get ':
      summary: Alerts Recipients
      description: Gets a information about alert recipient's targets.
      operationId: -alerts-recipients-recipient-id-
      x-api-path-slug: alertsrecipientsrecipient-id-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipient/{recipient_id} ':
    ' put ':
      summary: Alerts Recipient
      description: Updates recipient along with sms and email targets associated.
      operationId: -alerts-recipient-recipient-id-
      x-api-path-slug: alertsrecipientrecipient-id-put
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/recipient ':
    ' post ':
      summary: Alerts Recipient
      description: Creates a new recipient with one sms and one email target associated.
      operationId: -alerts-recipient-
      x-api-path-slug: alertsrecipient-post
      responses:
        200:
          description: OK
      tags:
      - Alerts
  '/alerts/targets ':
    ' get ':
      summary: Alerts Targets
      description: Gets a list of all alert targets that are visible to you as a customer.
      operationId: -alerts-targets-
      x-api-path-slug: alertstargets-get
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /alerts/configs/alertId:
    delete:
      summary: Deleting an alert
      description: Deleting an alert
      operationId: deleting-an-alert
      x-api-path-slug: alertsconfigsalertid-delete
      parameters:
      - in: path
        name: alertId
        description: The ID of the alert to be deleted
        type: string
      - in: path
        name: token
        description: Your API token
        type: string
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /alerts/configs/subjectId:
    get:
      summary: Listing alerts by subject
      description: Get a list of all configured alerts for a specific subject (device
        or service).
      operationId: listing-alerts-by-subject
      x-api-path-slug: alertsconfigssubjectid-get
      parameters:
      - in: path
        name: subjectId
        description: The ID of the subject e
        type: string
      - in: path
        name: subjectType
        description: The type of the subject - device or service
        type: string
      - in: query
        name: subjectType
        description: The type of the subject - device or service
        type: string
      - in: path
        name: token
        description: Your API token
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /alerts/triggered:
    get:
      summary: Triggered Alerts
      description: Get a list of all triggered alerts on your account, per subject
        (device or service) or per alert config.
      operationId: triggered-alerts
      x-api-path-slug: alertstriggered-get
      parameters:
      - in: query
        name: closed
        description: Whether to filter by closed or open alerts - unset = all alerts,
          false = open alerts, true = closed alerts
        type: string
      - in: query
        name: filter
        description: You can provide a JSON encoded hash filter for the search that
          will return items that match the filter
        type: string
      - in: query
        name: subjectType
        description: The type of the subject - device, service, deviceGroup or serviceGroup
          if you also specify the subjectId as part of the URL (see examples below)
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        200:
          description: OK
      tags:
      - Alerts
  /alerts/history/:
    "":
      summary: Listing costs
      description: |-
        Get the alerts history items limited by the given filter. If configId filter is set, then the results contains all events for that alert configuration. In any other case, the results are aggregated by itemId and configId including the following derived values:

        duration the sum of event durations.
        triggeredCount the number of events for that alert in that item.
        cost the HumanOps cost in seconds. For more information please check our support docs


        When the query is aggregated, the non-derived fields are from the document whose startDate is the newest. In addition to this, an unique id is generated by concatenating the itemId and the configId.
      operationId: listing-costs
      x-api-path-slug: alertshistory-
      parameters:
      - in: query
        name: configId
        description: _id of the config you want to limit by
        type: string
      - in: query
        name: end
        description: A string in the format, the end of the time frame eg
        type: string
      - in: query
        name: fields
        description: json encoded string - An array or a dict with all the fields
          we want returned
        type: string
      - in: query
        name: filter
        description: 'json encoded string - A dict with the filters we want to apply
          to the query (ex: {&quot;config'
        type: string
      - in: query
        name: order
        description: 'Sort ordering: ascending, descending'
        type: string
      - in: query
        name: page
        description: Page number, default = 1
        type: string
      - in: query
        name: perPage
        description: Documents that we&#39;re going to get per page
        type: string
      - in: query
        name: sort
        description: Field to sort by
        type: string
      - in: query
        name: start
        description: A string in the format, the beginning of the time frame eg
        type: string
      - in: query
        name: token
        description: Your API token
        type: string
      responses:
        "":
          description: ""
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Alerts
  /alerts/postbacks/:
    "":
      summary: Creating a postback
      description: You can use this method to post data back to Server Density without
        using the agent, for example using your own scripts or to integrate in something
        custom you are doing. You will still be restricted to posting back once per
        minute using this method, as you would be using the agent.
      operationId: creating-a-postback
      x-api-path-slug: alertspostbacks-
      parameters:
      - in: body
        name: hash
        description: An md5 hash of the JSON encoded payload, used for error checking
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: payload
        description: The payload you want to post back to us
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: token
        description: Your API token
        schema:
          $ref: '#/definitions/holder'
      - in: body
        name: X-Forwarded-Host
        description: Set this to your Server Density account url, e
        schema:
          $ref: '#/definitions/holder'
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
      tags:
      - Alerts
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