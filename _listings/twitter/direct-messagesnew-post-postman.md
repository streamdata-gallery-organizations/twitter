{
  "info": {
    "name": "Twitter Create Direct Message",
    "_postman_id": "ec1a3fc3-be5d-4025-b890-9386ca6d38b6",
    "description": "sends a new direct message to specified user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "7a875cc8-6651-4494-b057-86ba70da20d1",
          "name": "sends-a-new-direct-message-to-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/new?screen_name=%7B%7D&text=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sends a new direct message to specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5c616986-af3b-42bf-b121-eec6220878d4"
            }
          ]
        }
      ]
    }
  ]
}