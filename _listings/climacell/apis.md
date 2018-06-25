---
name: ClimaCell
x-slug: climacell
description: ClimaCell provides the most accurate weather data in the world by integrating
  proprietary data extracted from wireless networks and other new sensing technologies
  with data from traditional sensors. With 90% correlation to ground truth (vs. 50%
  using radar), it&rsquo;s the best you can get for your enterprise.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
x-kinRank: "9"
x-alexaRank: "617213"
tags: Alerts
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/climacell/apis.md
specificationVersion: "0.14"
apis:
- name: ClimaCell Get Alerts
  x-api-slug: climacell
  description: |-
    ### List all Alerts

    Page through a list of all your alerts. You can specify the maximum number of results to be retuned, and from which result to start.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//alerts
  tags: Weather,Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/climacell/alerts-get-openapi.md
- name: ClimaCell Post Alerts
  x-api-slug: climacell
  description: "### Create an Alert\nCreates a new Alert with the following information:\n\n*
    ```name``` - Alert Name\n* ```location_name``` - Location name for which the alert
    pertains (location has to be created earlier)\n* ```notice``` - Prior notice in
    seconds\n* ```conditions``` - logical expression defining a weather event such
    as: rain with intensity of more than 1 mm/hr. Several expressions can be concatenated
    with \u201Cor\u201D logical operator. An alert will trigger for it if any of its
    contained conditions are met. ORs can contain any number of conditions.\n\nNOTE:\u200B
    AND condition \u200B coming soon\n\n### In addition to the format below, this
    is an example with an \"OR\" conditional statement:\n  ```\n  {\n    \"name\":
    \"alert with or\",\n    \"location_name\": \"your-location-name\",\n    \"notice\":
    3600,\n    \"conditions\": [\n      {\n        \"or\": [\n          {\n            \"parameter\":
    \"Rain\",\n            \"value\": 0.15,\n            \"operator\": \"lt\"\n          },\n
    \         {\n            \"parameter\": \"Temperature\",\n            \"value\":
    25,\n            \"operator\": \"lt\"\n          }\n        ]\n      }\n    ],\n
    \   \"groups\": [\n      {\n        \"name\": \"your-group-name\",\n        \"delivery\":
    {\n          \"sms\": true,\n          \"email\": false\n        }\n      }\n
    \   ],\n    \"webhooks\": [507f1f77bcf86cd799439011]\n  }\n  ```\n### In addition
    to the format below, this is an example with an \"AND\" conditional statement:\n\n
    \ ```\n  {\n    \"name\": \"alert with AND conditions\",\n    \"location_name\":
    \"your-location-name\",\n    \"notice\": 3600,\n    \"conditions\": [\n      {\n
    \       \"parameter\": \"Rain\",\n        \"value\": 0.15,\n        \"operator\":
    \"gt\"\n      },\n      {\n        \"parameter\": \"Temperature\",\n        \"value\":
    40,\n        \"operator\": \"lt\"\n      }\n    ],\n    \"groups\": [\n      {\n
    \       \"name\": \"your-group-name\",\n        \"delivery\": {\n          \"sms\":
    true,\n          \"email\": false\n        }\n      }\n    ],\n    \"webhooks\":
    [507f1f77bcf86cd799439011]\n  }\n  ```"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//alerts
  tags: Weather,Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/climacell/alerts-post-openapi.md
- name: ClimaCell Get Alerts Alert
  x-api-slug: climacell
  description: |-
    ### Retrieve an Alert

    Get a single alert with its information by specifying its ```alert_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//alerts/{alert_id}
  tags: Weather,Alerts,Alert
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/climacell/alertsalert-id-get-openapi.md
- name: ClimaCell Put Alerts Alert
  x-api-slug: climacell
  description: |-
    ### Update an Alert

    Updates the details of an Alert designated by its ```alert_id```.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//alerts/{alert_id}
  tags: Weather,Alerts,Alert
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/climacell/alertsalert-id-put-openapi.md
- name: ClimaCell Delete Alerts Alert
  x-api-slug: climacell
  description: |-
    ### Delete an Alert

    Removes an alert with the ```alert_id``` from the system.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2//alerts/{alert_id}
  tags: Weather,Alerts,Alert
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/climacell/alertsalert-id-delete-openapi.md
- name: ClimaCell
  x-api-slug: climacell
  description: ClimaCell provides the most accurate weather data in the world by integrating
    proprietary data extracted from wireless networks and other new sensing technologies
    with data from traditional sensors. With 90% correlation to ground truth (vs.
    50% using radar), it&rsquo;s the best you can get for your enterprise.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28707-climacell.jpg
  humanURL: https://www.climacell.co
  baseURL: https://api2.climacell.co//v2
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/climacell/openapi.md
x-common:
- type: x-blog
  url: https://www.climacell.co/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/climacell
- type: x-developer
  url: https://www.climacell.co/api/
- type: x-email
  url: info@climacell.co
- type: x-email
  url: support@climacell.co
- type: x-email
  url: sales@climacell.co
- type: x-faq
  url: https://developer.climacell.co/FAQ
- type: x-github
  url: https://github.com/climacell
- type: x-pricing
  url: https://developer.climacell.co/
- type: x-privacy-policy
  url: https://www.climacell.co/privacy/
- type: x-terms-of-service
  url: https://www.climacell.co/terms-of-service/
- type: x-twitter
  url: https://twitter.com/WeatherRevealed
- type: x-website
  url: https://www.climacell.co
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---