{
  "info": {
    "name": "Stripe Get Events",
    "_postman_id": "729c9b14-fbce-44dd-99c7-31e7a3f6a7f5",
    "description": "Retrieves the details of an event. Supply the unique identifier of the event, which you might have received in a webhook.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "events",
      "item": [
        {
          "id": "3b42c167-f878-401b-a56d-db1702382641",
          "name": "getEvents",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "events/:id"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the details of an event"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f3207d6-df00-408f-b6a8-03eeb3ed9328"
            }
          ]
        }
      ]
    }
  ]
}