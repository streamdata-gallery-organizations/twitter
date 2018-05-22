{
  "info": {
    "name": "Twitter Add List Subscribers",
    "_postman_id": "905bf257-48bd-42ad-81bd-66b61a58d571",
    "description": "Subscribes the authenticated user to the specified list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "74d487cb-0be6-4862-b8e1-299d9cbb9ead",
          "name": "subscribes-the-authenticated-user-to-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/create?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Subscribes the authenticated user to the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8422bf8b-bbc9-4684-92c5-e7183b130b45"
            }
          ]
        }
      ]
    }
  ]
}