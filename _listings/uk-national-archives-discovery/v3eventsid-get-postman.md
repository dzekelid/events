{
  "info": {
    "name": "Getty Images Search API Get Events",
    "_postman_id": "694ebbb9-b56a-46de-978a-c0581d5e0805",
    "description": "Get metadata for a single event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "5a49418d-64b6-4a53-bfa4-f0300c9edd93",
          "name": "getV3Events",
          "request": {
            "url": "http://api.gettyimages.com/v3/events?fields=%7B%7D&ids=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept-Language",
                "value": "{}",
                "description": "Specifies the language of result values",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Provide access token in the format of Bearer {token}",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get metadata for multiple events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac39f89c-6a06-495f-b869-dd923daa77c5"
            }
          ]
        },
        {
          "id": "a3bf71fa-635a-497e-8b9f-33f503c6163e",
          "name": "getV3Events",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.gettyimages.com",
              "path": [
                "v3/events/:id"
              ],
              "query": [
                {
                  "key": "fields",
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
            "header": [
              {
                "key": "Accept-Language",
                "value": "{}",
                "description": "Specifies the language of result values",
                "disabled": false
              },
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Provide access token in the format of Bearer {token}",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get metadata for a single event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8499768d-5b7d-4b6d-9e01-7dfb03a30be5"
            }
          ]
        }
      ]
    }
  ]
}