{
  "info": {
    "name": "Twitter Show List Subscriptions",
    "_postman_id": "9b721042-067d-436c-8c1c-62f9dd8fb024",
    "description": "Returns list of subscriptions",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "ff122b10-e647-4c73-ad62-68ed477d3cd5",
          "name": "returns-list-of-subscriptions",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscriptions?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of subscriptions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43acc609-b82d-410a-841d-15a893e04a71"
            }
          ]
        }
      ]
    }
  ]
}