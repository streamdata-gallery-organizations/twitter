{
  "info": {
    "name": "Twitter Get Sent Direct Messages",
    "_postman_id": "20e401a9-f8c4-4d55-af5b-f4935826d50c",
    "description": "return 20 most recent direct messages sent",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "db7128a9-0aeb-4a70-a4d4-aba7e011061a",
          "name": "return-20-most-recent-direct-messages-sent",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/sent?count=%7B%7D&include_entities=%7B%7D&max_id=%7B%7D&page=%7B%7D&since_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "return 20 most recent direct messages sent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34f46a29-164d-46a3-a9c4-d2e3e4dfe8c0"
            }
          ]
        }
      ]
    }
  ]
}