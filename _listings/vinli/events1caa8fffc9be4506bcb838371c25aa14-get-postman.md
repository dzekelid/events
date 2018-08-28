{
  "info": {
    "name": "Vinli Get a Specific Event",
    "_postman_id": "a30d4961-b760-4573-b21f-e28beb5efe61",
    "description": "Get a specific event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Eventsa",
      "item": [
        {
          "id": "34bb26ae-6a32-4697-ac26-72313fc7f5d3",
          "name": "Devices62976d30B6dc40f18422Ccc367572101EventsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/devices/62976d30-b6dc-40f1-8422-ccc367572101/events",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all events for a device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8db50297-6490-4182-9fef-2a8865a97ebb"
            }
          ]
        }
      ]
    },
    {
      "name": "Specific",
      "item": [
        {
          "id": "8cad92bf-f29b-4b79-9d98-d3bdb6680d05",
          "name": "Events1caa8fffC9be4506Bcb838371c25aa14Get",
          "request": {
            "url": "http://events.vin.li/api/v1/events/1caa8fff-c9be-4506-bcb8-38371c25aa14",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a specific event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e394265-8053-4372-aea2-879f709815a4"
            }
          ]
        }
      ]
    },
    {
      "name": "Notificationsan",
      "item": [
        {
          "id": "cc32f422-3a6b-44e7-b25f-2080a06027a8",
          "name": "EventsD69cc8beA809441d8a701bf0a0d48fb3NotificationsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/events/d69cc8be-a809-441d-8a70-1bf0a0d48fb3/notifications",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get notifications for an event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d75aa65-c570-4c9b-bede-50636ccb17c1"
            }
          ]
        }
      ]
    }
  ]
}