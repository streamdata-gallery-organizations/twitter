{
  "info": {
    "name": "Twitter Show Closes Trends",
    "_postman_id": "95f1563e-19aa-4b8a-8676-84b90a0416a9",
    "description": "Returns the location that Twitter has trending topic information for",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "ab1a928f-a0a8-4471-82e0-3ff14011b31f",
          "name": "returns-the-location-that-twitter-has-trending-topic-information-for",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/closest.json?lat=%7B%7D&long=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the location that Twitter has trending topic information for"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eae308e6-c782-4556-8785-a10b76c8b404"
            }
          ]
        }
      ]
    }
  ]
}