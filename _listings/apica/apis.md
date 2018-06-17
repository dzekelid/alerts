---
name: Apica
x-slug: apica
description: Apica???s performance testing and monitoring solutions provide critical
  peak performance data and 24/7 monitoring of applications and sites around the world.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
x-kinRank: "7"
x-alexaRank: "827487"
tags: Alerts
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/apis.md
specificationVersion: "0.14"
apis:
- name: Alerts API Alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id}
  x-api-slug: alerts-api
  description: Gets alerts filtered by set of optional parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts?check_id={check_id}&amp;severity={severity}&amp;enabled={enabled}&amp;target_type={target_type}&amp;target_id={target_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertscheck-idcheck-idampseverityseverityampenabledenabledamptarget-typetarget-typeamptarget-idtarget-id-get-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Gets alert by Id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsalert-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsalert-id-get-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Updates alert.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsalert-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsalert-id-put-openapi.md
- name: Alerts API Alerts {alert_id}
  x-api-slug: alerts-api
  description: Deletes alert by Id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/{alert_id} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsalert-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsalert-id-delete-openapi.md
- name: Alerts API Alerts {alert_type}
  x-api-slug: alerts-api
  description: Creates a new alert.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/{alert_type} '
  tags: Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsalert-type-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsalert-type-post-openapi.md
- name: Alerts API Alerts Recipients
  x-api-slug: alerts-api
  description: Gets a list of all alert recipient's targets that are visible to you
    as a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/recipients '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsrecipients-get-openapi.md
- name: Alerts API Alerts Recipients {recipient_id}
  x-api-slug: alerts-api
  description: Gets a information about alert recipient's targets.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/recipients/{recipient_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsrecipientsrecipient-id-get-openapi.md
- name: Alerts API Alerts Recipient {recipient_id}
  x-api-slug: alerts-api
  description: Updates recipient along with sms and email targets associated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/recipient/{recipient_id} '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsrecipientrecipient-id-put-openapi.md
- name: Alerts API Alerts Recipient
  x-api-slug: alerts-api
  description: Creates a new recipient with one sms and one email target associated.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/recipient '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsrecipient-post-openapi.md
- name: Alerts API Alerts Targets
  x-api-slug: alerts-api
  description: Gets a list of all alert targets that are visible to you as a customer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: '://api.serverdensity.io.///alerts/targets '
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertstargets-get-openapi.md
- name: Alerts API Deleting an alert
  x-api-slug: alerts-api
  description: Deleting an alert
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: ://api.serverdensity.io.///alerts/configs/alertId
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsconfigsalertid-delete-openapi.md
- name: Alerts API Listing alerts by subject
  x-api-slug: alerts-api
  description: Get a list of all configured alerts for a specific subject (device
    or service).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: ://api.serverdensity.io.///alerts/configs/subjectId
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertsconfigssubjectid-get-openapi.md
- name: Alerts API Triggered alerts
  x-api-slug: alerts-api
  description: Get a list of all triggered alerts on your account, per subject (device
    or service) or per alert config.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: ://api.serverdensity.io.///alerts/triggered
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/alertstriggered-get-openapi.md
- name: Alerts API
  x-api-slug: alerts-api
  description: Apica???s performance testing and monitoring solutions provide critical
    peak performance data and 24/7 monitoring of applications and sites around the
    world.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/19004-apica.jpg
  humanURL: https://www.apicasystem.com
  baseURL: ://api.serverdensity.io./
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/apica/openapi.md
x-common:
- type: x-blog
  url: https://www.apicasystem.com/blog/
- type: x-blog-rss
  url: https://www.apicasystem.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/apica
- type: x-developer
  url: http://api-wpm.apicasystem.com/v3/help
- type: x-documentation
  url: https://api-wpm.apicasystem.com/v3/Help
- type: x-email
  url: sales@apicasystems.com
- type: x-email
  url: swesales@apicasystems.com
- type: x-email
  url: support@apicasystems.com
- type: x-email
  url: operations@apicasystem.com
- type: x-github
  url: https://github.com/ApicaSystem
- type: x-twitter
  url: https://twitter.com/apicasystems
- type: x-website
  url: https://www.apicasystem.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---