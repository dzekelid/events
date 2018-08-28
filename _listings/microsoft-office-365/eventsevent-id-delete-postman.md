{
  "info": {
    "name": "Microsoft Office 365 Delete Events Event",
    "_postman_id": "061be0a1-6179-4e2e-83c6-88abc49ab642",
    "description": "Upon success, the appointment is moved to the user's Deleted...",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "events",
      "item": [
        {
          "id": "54067b3b-68a1-453a-8485-0aa18040a9b4",
          "name": "deleteEventsEvent",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Upon success, the appointment is moved to the user's Deleted"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e63daed-9bad-4e57-bf1b-c3ea3c8c0a28"
            }
          ]
        }
      ]
    }
  ]
}