{
  "info": {
    "name": "Twitter Show Place Trends",
    "_postman_id": "1cf725b6-d5e1-4604-8fb7-91a5cd4fe8e8",
    "description": "Returns the top 10 trending topics for a specific WOEID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "53fe73ac-d420-42a7-adf6-3419ddaea939",
          "name": "returns-the-top-10-trending-topics-for-a-specific-woeid",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/place.json?exclude=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top 10 trending topics for a specific WOEID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78ce6200-c968-4078-8a32-b0234e595e2b"
            }
          ]
        }
      ]
    }
  ]
}