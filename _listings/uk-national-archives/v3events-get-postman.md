{
  "info": {
    "name": "Getty Images Search API Get Events",
    "_postman_id": "78919e43-6bd5-4c61-83b8-5f990df145db",
    "description": "Get metadata for multiple events.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "7e782630-ba4e-4b92-8470-f7babbe0fc3a",
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
              "id": "f5cf5b86-55c8-49c7-9853-d4fdc3b00e53"
            }
          ]
        }
      ]
    }
  ]
}