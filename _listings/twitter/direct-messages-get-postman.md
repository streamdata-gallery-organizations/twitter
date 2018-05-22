{
  "info": {
    "name": "Twitter Get Direct Messages",
    "_postman_id": "712d0844-cd0a-4ed7-a81a-59309e7f1473",
    "description": "return 20 most recent direct messages sent to user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "311a1ce9-f7c5-4b01-b604-b310a9493f76",
          "name": "return-20-most-recent-direct-messages-sent-to-user",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages?include_entities=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&skip_status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "return 20 most recent direct messages sent to user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8332407c-e44e-4061-8193-71f1eb9cf3eb"
            }
          ]
        }
      ]
    }
  ]
}