{
  "info": {
    "name": "AXA Assistance Retrieve the latest alerts worldwide",
    "_postman_id": "a71f8ebc-55dd-48ec-930d-6b89a5db559f",
    "description": "Retrieve the latest alerts worldwide",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "f86c9206-0d53-4971-8d62-bcc250bcc5d4",
          "name": "getInformationV1CountriesAlerts",
          "request": {
            "url": "http://sandbox.api.axa-assistance.com/information/v1/countries/alerts",
            "method": "GET",
            "header": [
              {
                "key": "accept-language",
                "value": "{}",
                "description": "Language/Country",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the latest alerts worldwide"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04e2e957-e727-44a3-906d-d61ad7ddca11"
            }
          ]
        }
      ]
    }
  ]
}