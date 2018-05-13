{
  "info": {
    "name": "Azure Activity Log Alerts API",
    "_postman_id": "1ae59fda-23ae-4b93-930a-13c966baeceb",
    "description": "",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "activity log alerts subscription id",
      "item": [
        {
          "id": "7ef6c7ba-3b54-4b79-a084-c87d2ef19e65",
          "name": "ActivityLogAlerts_ListBySubscriptionId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/microsoft.insights/activityLogAlerts"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all activity log alerts in a subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ee8dc9b-35b7-4be8-802a-b8f87c03100a"
            }
          ]
        }
      ]
    }
  ]
}