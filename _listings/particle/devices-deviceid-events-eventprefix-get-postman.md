{
  "info": {
    "name": "Particle Get Devices Device Events",
    "_postman_id": "b30e2a12-7faa-4818-a7af-4cdf695676ce",
    "description": "Open a stream of Server Sent Events for all public events and private events for your devices.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "devices",
      "item": [
        {
          "id": "f819f106-f192-4a3c-a292-56f6831f7f45",
          "name": "getDevicesDeviceEventsEventprefix",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.particle.io",
              "path": [
                "v1",
                "devices/:deviceID/events/:eventPrefix"
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
                  "id": "deviceID",
                  "value": "deviceID",
                  "type": "string"
                },
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
              "id": "0d4d74fc-996f-4007-bdc7-18073393871a"
            }
          ]
        }
      ]
    }
  ]
}