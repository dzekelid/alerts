---
name: Azure Monitor
description: Autoscale is a built-in feature of Cloud Services, Mobile Services, Virtual
  Machines, and Websites that helps applications perform their best when demand changes.
  Of course, performance means different things for different applications. Some apps
  are CPU-bound, others memory-bound. For example, you could have a web app that handles
  millions of requests during the day and none at night. Autoscale can scale your
  service by any of thesemdash;or by a custom metric you define.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
x-kinRank: "10"
x-alexaRank: ""
tags:
- Stack Network
- Monitoring
- Microsoft
- Cloud
created: "2018-05-12"
modified: "2018-05-12"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/apis.yaml
specificationVersion: "0.14"
apis:
- name: Azure Activity Log API
  description: Autoscale is a built-in feature of Cloud Services, Mobile Services,
    Virtual Machines, and Websites that helps applications perform their best when
    demand changes
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
  humanURL: ""
  baseURL: ://management.azure.com//
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-insights-activitylogalerts-activitylogalertname-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptions-subscriptionid-resourcegroups-resourcegroupname-providers-microsoft-insights-activitylogalerts-activitylogalertname-get-postman.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/monitor/
- type: x-service-level-agreement
  url: https://azure.microsoft.com/en-us/support/legal/sla/monitor/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/monitor/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---