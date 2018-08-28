{
  "info": {
    "name": "Kubernetes Get Events",
    "_postman_id": "b3070d55-a256-41ac-956b-ec26660dacd0",
    "description": "List objects of kind event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "5f0738c0-49dd-4104-8267-f48a365bc32b",
          "name": "listEvent",
          "request": {
            "url": "http:///api/v1beta3/127.0.0.1:6443/api/v1beta3/events",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List objects of kind event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e24aeed-bfaf-428f-a177-1f37e07762ae"
            }
          ]
        }
      ]
    }
  ]
}