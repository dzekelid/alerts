---
name: Azure Monitor
x-slug: azure-monitor
description: Autoscale is a built-in feature of Cloud Services, Mobile Services, Virtual
  Machines, and Websites that helps applications perform their best when demand changes.
  Of course, performance means different things for different applications. Some apps
  are CPU-bound, others memory-bound. For example, you could have a web app that handles
  millions of requests during the day and none at night. Autoscale can scale your
  service by any of these&mdash;or by a custom metric you define.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
x-kinRank: "10"
x-alexaRank: "0"
tags: Alerts
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/apis.md
specificationVersion: "0.14"
apis:
- name: Azure Activity Log API Activity Log Alerts Create Or Update
  x-api-slug: azure-activity-log-api
  description: Create a new activity log alert or update an existing one.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
  humanURL: https://azure.microsoft.com/en-us/services/monitor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/activityLogAlerts/{activityLogAlertName}
  tags: Activity Log Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalertsactivitylogalertname-put-openapi.md
- name: Azure Activity Log API Activity Log Alerts Get
  x-api-slug: azure-activity-log-api
  description: Get an activity log alert.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
  humanURL: https://azure.microsoft.com/en-us/services/monitor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/activityLogAlerts/{activityLogAlertName}
  tags: Activity Log Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalertsactivitylogalertname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalertsactivitylogalertname-get-openapi.md
- name: Azure Activity Log API Activity Log Alerts Delete
  x-api-slug: azure-activity-log-api
  description: Delete an activity log alert.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
  humanURL: https://azure.microsoft.com/en-us/services/monitor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/activityLogAlerts/{activityLogAlertName}
  tags: Activity Log Alerts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalertsactivitylogalertname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalertsactivitylogalertname-delete-openapi.md
- name: Azure Activity Log API Activity Log Alerts Update
  x-api-slug: azure-activity-log-api
  description: Updates an existing ActivityLogAlertResource's tags. To update other
    fields use the CreateOrUpdate method.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
  humanURL: https://azure.microsoft.com/en-us/services/monitor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/activityLogAlerts/{activityLogAlertName}
  tags: Activity Log Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalertsactivitylogalertname-patch-openapi.md
- name: Azure Activity Log API Activity Log Alerts List By Subscription Id
  x-api-slug: azure-activity-log-api
  description: Get a list of all activity log alerts in a subscription.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
  humanURL: https://azure.microsoft.com/en-us/services/monitor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/microsoft.insights/activityLogAlerts
  tags: Activity Log Alerts Subscription Id
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidprovidersmicrosoft-insightsactivitylogalerts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidprovidersmicrosoft-insightsactivitylogalerts-get-openapi.md
- name: Azure Activity Log API Activity Log Alerts List By Resource Group
  x-api-slug: azure-activity-log-api
  description: Get a list of all activity log alerts in a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
  humanURL: https://azure.microsoft.com/en-us/services/monitor/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/microsoft.insights/activityLogAlerts
  tags: Activity Log Alerts Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalerts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-insightsactivitylogalerts-get-openapi.md
- name: Azure Activity Log API
  x-api-slug: azure-activity-log-api
  description: Autoscale is a built-in feature of Cloud Services, Mobile Services,
    Virtual Machines, and Websites that helps applications perform their best when
    demand changes. Of course, performance means different things for different applications.
    Some apps are CPU-bound, others memory-bound. For example, you could have a web
    app that handles millions of requests during the day and none at night. Autoscale
    can scale your service by any of these&mdash;or by a custom metric you define.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/manage-monitoring-data.png
  humanURL: https://azure.microsoft.com/en-us/services/monitor/
  baseURL: ://management.azure.com//
  tags: Alerts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/alerts/master/_listings/azure-monitor/openapi.md
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