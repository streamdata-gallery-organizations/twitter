{
  "info": {
    "name": "Twitter Geo Search",
    "_postman_id": "46770d71-61cb-4b34-af32-b9ad5d7ed83f",
    "description": "Search for places that can be attached to a statuses/updates",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "places",
      "item": [
        {
          "id": "7552be25-89a9-4bff-b847-cbe3e2dd5900",
          "name": "search-for-places-that-can-be-attached-to-a-statusesupdates",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/search?accuracy=%7B%7D&attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&granularity=%7B%7D&ip=%7B%7D&lat=%7B%7D&long=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for places that can be attached to a statuses/updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "baff0153-0570-4f85-8755-269c98d707d7"
            }
          ]
        }
      ]
    }
  ]
}