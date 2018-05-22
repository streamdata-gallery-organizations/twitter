{
  "info": {
    "name": "Twitter Update List",
    "_postman_id": "baff3ffa-a83d-4df8-9f2d-e1be527a0c80",
    "description": "Returns lists of updates",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "a8d022fd-16b5-4183-95dc-32f3ae31437b",
          "name": "returns-lists-of-updates",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/update?description=%7B%7D&list_id=%7B%7D&mode=%7B%7D&name=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "538fd2d5-fcd5-4c3a-aa98-b8fdd995b0a8"
            }
          ]
        }
      ]
    }
  ]
}