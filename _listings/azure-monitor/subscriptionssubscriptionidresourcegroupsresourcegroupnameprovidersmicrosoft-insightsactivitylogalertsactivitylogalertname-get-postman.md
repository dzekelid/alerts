{
  "info": {
    "name": "Azure Activity Log Alerts API",
    "_postman_id": "0db1e84b-ba97-470a-bca9-0957017e2522",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "activity log alerts",
      "item": [
        {
          "id": "d7c2e99b-2d24-4be8-82e8-d70721b2d37e",
          "name": "ActivityLogAlerts_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/microsoft.insights/activityLogAlerts/:activityLogAlertName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "activityLogAlertName",
                  "value": "activityLogAlertName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get an activity log alert"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec91ff0d-0772-4e55-bfcf-c937a8b7756c"
            }
          ]
        }
      ]
    }
  ]
}