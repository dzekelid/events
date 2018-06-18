{
  "info": {
    "name": "Lota Data Get Events",
    "_postman_id": "7f0a1613-917f-41a0-a7c8-c56b3eb8c84b",
    "description": "Find event occurrences in the area. returns results at specific place and time, event groups are expanded for every occurrence..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Events",
      "item": [
        {
          "id": "20345b88-1889-40cb-b25f-74f6463608d5",
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
              "id": "85a375c4-073d-4104-99c9-ad82dc41e4da"
            }
          ]
        }
      ]
    }
  ]
}