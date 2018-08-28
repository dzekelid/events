{
  "info": {
    "name": "Shopify Count all the events",
    "_postman_id": "7ee96a0f-9920-4e43-a3d8-d90bbad52331",
    "description": "Count all the events.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "6cf33b35-5874-4bd9-becc-e74a544314f9",
          "name": "getAdminOrders4554953422Events.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/orders/4554953422/events.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all the events from a particular order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0724b15-6ee9-4335-878f-0a6fb0ef15a3"
            }
          ]
        },
        {
          "id": "110dfa5c-a9d5-494d-a2a6-e939282a1244",
          "name": "getAdminProducts7990943555Events.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/products/7990943555/events.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all the events from a particular product."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed4beb5d-5599-4381-a89d-1b4159ac2b14"
            }
          ]
        },
        {
          "id": "73cb95a5-b86e-40be-9779-b570b5c3bcc7",
          "name": "getAdminEventsCount.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/events/count.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Count all the events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bde4b25-be7d-49a1-b6b8-370c3ff93372"
            }
          ]
        }
      ]
    }
  ]
}