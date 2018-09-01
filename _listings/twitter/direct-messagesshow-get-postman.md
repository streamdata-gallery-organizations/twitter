{
  "info": {
    "name": "Twitter Show Direct Message",
    "_postman_id": "fbc3e1c9-8e97-45d6-aa51-d44c12cec28a",
    "description": "returns a single direct message specified by an id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "dbadf40a-18a5-4781-b767-07f4b4ef17f3",
          "name": "returns-a-single-direct-message-specified-by-an-id",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/show?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a single direct message specified by an id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aafa2f8b-d64a-4211-90c4-047f051af6ec"
            }
          ]
        }
      ]
    }
  ]
}