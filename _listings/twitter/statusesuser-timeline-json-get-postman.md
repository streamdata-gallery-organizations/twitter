{
  "info": {
    "name": "Twitter Show Timelines Status",
    "_postman_id": "840f5a8a-2c8c-4bbe-80e5-0c2829d01af7",
    "description": "Returns a collection of the most recent Tweets posted by the User",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "457f15d4-24ec-46a5-ad63-626fbcad86ad",
          "name": "returns-a-collection-of-the-most-recent-tweets-posted-by-the-user",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/user_timeline.json?contributor_details=%7B%7D&count=%7B%7D&exclude_replies=%7B%7D&include_rts=%7B%7D&max_id=%7B%7D&screen_name=screen_name&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of the most recent Tweets posted by the User"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5d1bc5c-27ad-41c9-8bf1-7088e74f59fb"
            }
          ]
        }
      ]
    }
  ]
}