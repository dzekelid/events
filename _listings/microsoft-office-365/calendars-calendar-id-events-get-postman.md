{
  "info": {
    "name": "Microsoft Office 365 Get Calendars Calendar Events",
    "_postman_id": "a0f5260a-2439-4222-8406-3f65f1d32e9b",
    "description": "You can request all the events across all calendars (or a fi...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "calendars",
      "item": [
        {
          "id": "408c635a-9e35-45ac-94f8-88499fce046e",
          "name": "getCalendarsCalendarEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "outlook.office365.com",
              "path": [
                "ews",
                "odata",
                "Me",
                "Calendars:calendar_id/Events"
              ],
              "variable": [
                {
                  "id": "calendar_id",
                  "value": "calendar_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "You can request all the events across all calendars (or a fi"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d7dd1c3-19fc-484e-ad05-77ab8510ee31"
            }
          ]
        }
      ]
    }
  ]
}