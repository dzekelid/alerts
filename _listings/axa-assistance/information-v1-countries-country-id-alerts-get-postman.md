{
  "info": {
    "name": "AXA Assistance",
    "_postman_id": "2aa6997a-e4ba-4212-b8c2-d26864bd5216",
    "description": "AXA Assistance is a worldwide specialist for car insurance, travel, health and home services. Trust in Axa Assistance for your insurance!",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "insurance",
      "item": [
        {
          "id": "902a7bd7-d104-4795-acd0-5ff2413d74c8",
          "name": "getInformationV1CountriesCountry_idAlerts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "sandbox.api.axa-assistance.com",
              "path": [
                "information/v1/countries/:country_id/alerts"
              ],
              "variable": [
                {
                  "id": "country_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Retrieve the latest alerts for a specified country"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ef15cbc-7de4-4671-969d-5cc8322e6e67"
            }
          ]
        }
      ]
    }
  ]
}