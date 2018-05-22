{
  "info": {
    "name": "Twitter Mentions Timelines",
    "_postman_id": "22c8b185-ae92-4371-8f5d-38a198a98465",
    "description": "Returns the 20 most recent mentions for the authenticating user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "26919527-225f-41c1-b55d-7b18823b4fe4",
          "name": "returns-the-20-most-recent-mentions-for-the-authenticating-user",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/mentions_timeline?contributor_details=%7B%7D&count=%7B%7D&include_entities=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the 20 most recent mentions for the authenticating user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "247ae5bd-b26e-45bf-a2bf-6bfbde9e386f"
            }
          ]
        }
      ]
    }
  ]
}