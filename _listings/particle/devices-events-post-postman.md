{
  "info": {
    "name": "Particle Add Devices Events",
    "_postman_id": "c49bbb2f-eabe-40b5-89e4-29805c375f75",
    "description": "Publish an event",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "c6e71c8f-6e66-4d34-8d42-a9b49f735dc6",
          "name": "postDevicesEvents",
          "request": {
            "url": "http://api.particle.io/v1/devices/events",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "data",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event data"
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": "Event name"
                },
                {
                  "key": "private",
                  "value": "{}",
                  "disabled": false,
                  "description": "If you wish this event to be publicly visible"
                },
                {
                  "key": "ttl",
                  "value": "{}",
                  "disabled": false,
                  "description": "How long the event should persist"
                }
              ]
            },
            "description": "Publish an event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a6c735a-afa8-4efa-b741-475233a34c7e"
            }
          ]
        }
      ]
    }
  ]
}