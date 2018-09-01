{
  "info": {
    "name": "Twitter Get Similar Places",
    "_postman_id": "04bef8dd-fb33-4c1e-b4fb-34023ab61049",
    "description": "Locates places near the given coordinates which are similar in name",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "places",
      "item": [
        {
          "id": "9ff630ff-e914-44fe-a963-c5c478481d03",
          "name": "locates-places-near-the-given-coordinates-which-are-similar-in-name",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/similar_places?attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&lat=%7B%7D&long=%7B%7D&name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Locates places near the given coordinates which are similar in name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13f0e084-9109-42b0-b1d0-54ed6c0a9662"
            }
          ]
        }
      ]
    }
  ]
}