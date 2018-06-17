{
  "info": {
    "name": "Azure Activity Log Alerts API",
    "_postman_id": "e5af0258-e31f-4db3-92ef-190d56b0e63b",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "activity log alerts",
      "item": [
        {
          "id": "e5aec252-c8fd-4e94-a415-65178cbabcec",
          "name": "ActivityLogAlerts_Delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an activity log alert"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "732e6e3b-7a4c-4db9-90ad-f193774917f1"
            }
          ]
        }
      ]
    }
  ]
}