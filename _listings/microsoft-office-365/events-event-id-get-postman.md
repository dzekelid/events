{
  "info": {
    "name": "Microsoft Office 365 Get Events Event",
    "_postman_id": "1106394b-318f-436c-8aab-4f6c8eeec386",
    "description": "You can also retrieve information about a specific event by ...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "events",
      "item": [
        {
          "id": "0d4ec4e7-c3b5-44ba-985a-880cbe0c2d42",
          "name": "getEventsEvent",
          "request": {
            "url": {
              "protocol": "http",
              "host": "outlook.office365.com",
              "path": [
                "ews",
                "odata",
                "Me",
                "Events:event_id"
              ],
              "variable": [
                {
                  "id": "event_id",
                  "value": "event_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can also retrieve information about a specific event by "
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84088e3d-62cb-4a0c-a9da-8ce99e65cb8f"
            }
          ]
        }
      ]
    }
  ]
}