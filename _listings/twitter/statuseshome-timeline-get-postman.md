{
  "info": {
    "name": "Twitter Status Timeline",
    "_postman_id": "85bb0f25-9384-457e-b603-e4afa16dc452",
    "description": "Returns a collection of the most recent Tweets",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "a9b4b518-6b42-45a0-8a49-6b619eca2943",
          "name": "returns-a-collection-of-the-most-recent-tweets",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/home_timeline?contributor_details=%7B%7D&exclude_replies=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of the most recent Tweets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f28147b6-9f62-4289-b1f8-4a32bf9137e9"
            }
          ]
        }
      ]
    }
  ]
}