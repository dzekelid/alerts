---
name: Pingometer
x-slug: pingometer
description: Pingometer is a service that monitors the uptime, downtime, and performance
  of websites. Get 24/7 monitoring - sign up for your FREE account today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
x-kinRank: "8"
x-alexaRank: "1995680"
tags: Alerts
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/apis.md
specificationVersion: "0.14"
apis:
- name: Alerts API Alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id}
  x-api-slug: alerts-api
  description: Gets alerts filtered by set of optional parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertscheck-idcheck-idampseverityseverityampenabledenabledamptarget-typetarget-typeamptarget-idtarget-id-get-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Gets alert by Id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsalert-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsalert-id-get-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Updates alert.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsalert-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsalert-id-put-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Deletes alert by Id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsalert-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsalert-id-delete-openapi.md
- name: Alerts API Alerts {alert_type}
  x-api-slug: alerts-api
  description: Creates a new alert.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/{alert_type} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsalert-type-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsalert-type-post-openapi.md
- name: Alerts API Alerts Recipients
  x-api-slug: alerts-api
  description: Gets a list of all alert recipient's targets that are visible to you
    as a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/recipients '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsrecipients-get-openapi.md
- name: Alerts API Alerts Recipients {recipient_id}
  x-api-slug: alerts-api
  description: Gets a information about alert recipient's targets.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/recipients/{recipient_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsrecipientsrecipient-id-get-openapi.md
- name: Alerts API Alerts Recipient {recipient_id}
  x-api-slug: alerts-api
  description: Updates recipient along with sms and email targets associated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/recipient/{recipient_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsrecipientrecipient-id-put-openapi.md
- name: Alerts API Alerts Recipient
  x-api-slug: alerts-api
  description: Creates a new recipient with one sms and one email target associated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/recipient '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsrecipient-post-openapi.md
- name: Alerts API Alerts Targets
  x-api-slug: alerts-api
  description: Gets a list of all alert targets that are visible to you as a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: '://api.serverdensity.io.///alerts/targets '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertstargets-get-openapi.md
- name: Alerts API Deleting an alert
  x-api-slug: alerts-api
  description: Deleting an alert
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: ://api.serverdensity.io.///alerts/configs/alertId
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsconfigsalertid-delete-openapi.md
- name: Alerts API Listing alerts by subject
  x-api-slug: alerts-api
  description: Get a list of all configured alerts for a specific subject (device
    or service).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: ://api.serverdensity.io.///alerts/configs/subjectId
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertsconfigssubjectid-get-openapi.md
- name: Alerts API Triggered alerts
  x-api-slug: alerts-api
  description: Get a list of all triggered alerts on your account, per subject (device
    or service) or per alert config.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: ://api.serverdensity.io.///alerts/triggered
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/alertstriggered-get-openapi.md
- name: Alerts API
  x-api-slug: alerts-api
  description: Pingometer is a service that monitors the uptime, downtime, and performance
    of websites. Get 24/7 monitoring - sign up for your FREE account today!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18847-pingometer.jpg
  humanURL: https://pingometer.com/
  baseURL: ://api.serverdensity.io./
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/pingometer/openapi.md
x-common:
- type: x-blog
  url: https://pingometer.com/blog/
- type: x-crunchbase
  url: https://www.crunchbase.com/organization/pingometer
- type: x-crunchbase
  url: https://crunchbase.com/organization/pingometer
- type: x-github
  url: https://github.com/pingometer
- type: x-integrations
  url: https://pingometer.com/integrations/
- type: x-twitter
  url: https://twitter.com/pingometer
- type: x-website
  url: https://pingometer.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---