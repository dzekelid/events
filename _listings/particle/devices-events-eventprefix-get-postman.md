{
  "info": {
    "name": "Particle Get Devices Events",
    "_postman_id": "803f53a8-e2d7-43d2-b07d-b673a8b594d6",
    "description": "Open a stream of Server Sent Events for all public events and private events for your devices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "7b839994-8d0d-4060-8d03-2eac435a2acc",
          "name": "getDevicesEventsEventprefix",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.particle.io",
              "path": [
                "v1",
                "devices/events/:eventPrefix"
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
                  "id": "eventPrefix",
                  "value": "eventPrefix",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Open a stream of Server Sent Events for all public events and private events for your devices"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6269f593-8767-47fd-be1a-9aa33cf5f0f6"
            }
          ]
        }
      ]
    }
  ]
}