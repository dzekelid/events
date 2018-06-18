{
  "info": {
    "name": "Lota Data Get Events",
    "_postman_id": "774c1c19-e708-45cc-a165-43d52527d945",
    "description": "Get specific event details..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "68aecc8d-a55d-4a5a-be33-cb990081945a",
          "name": "events.get",
          "request": {
            "url": "http://api2.lotadata.com/v2/events?activity=%7B%7D&ambience=%7B%7D&bbox=%7B%7D&capacity_max=%7B%7D&capacity_min=%7B%7D&category=%7B%7D&center=%7B%7D&fieldset=%7B%7D&from_day=%7B%7D&genre=%7B%7D&limit=%7B%7D&name=%7B%7D&offset=%7B%7D&polygon=%7B%7D&q=%7B%7D&radius=%7B%7D&to_day=%7B%7D&within=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Find event occurrences in the area. returns results at specific place and time, event groups are expanded for every occurrence.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1133f790-ca65-4770-a29d-e60a5ecb7f7a"
            }
          ]
        },
        {
          "id": "f8f1e727-5a31-42b7-a963-17127949e89a",
          "name": "events.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api2.lotadata.com",
              "path": [
                "v2",
                "events/:id"
              ],
              "query": [
                {
                  "key": "fieldset",
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
            "description": "Get specific event details.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59b664a9-99e7-4f7e-b6d7-774917d84fbd"
            }
          ]
        }
      ]
    }
  ]
}