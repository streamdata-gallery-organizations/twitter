{
  "info": {
    "name": "Twitter Destroy List",
    "_postman_id": "b78eb68a-1ed6-4dd3-8477-c60b8016e001",
    "description": "Returns list of destroy",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "73441e01-6386-4525-94d0-c8195195311b",
          "name": "returns-list-of-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2834028d-b29c-4793-9b13-55578f4b05c5"
            }
          ]
        }
      ]
    }
  ]
}