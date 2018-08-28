{
  "info": {
    "name": "Vinli Get All Events for a Device",
    "_postman_id": "dcab6b26-764c-403a-b4ae-a2a9d2526fda",
    "description": "Get all events for a device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Eventsa",
      "item": [
        {
          "id": "6d437733-a2e8-4a47-9a36-456741974804",
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
              "id": "2ac91e5c-e2c4-4e2b-bb66-9127b1bdf3f0"
            }
          ]
        }
      ]
    },
    {
      "name": "Specific",
      "item": [
        {
          "id": "3e0b3544-bfa5-4b81-9c49-c5869b1ce522",
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
              "id": "f838512a-a5d6-4df1-b830-6bdf1a72a910"
            }
          ]
        }
      ]
    },
    {
      "name": "Notificationsan",
      "item": [
        {
          "id": "ccdfb06d-f3cf-4f76-8d6f-68734756405f",
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
              "id": "edd4144c-79ed-48bc-b96a-a06d0142166f"
            }
          ]
        }
      ]
    }
  ]
}