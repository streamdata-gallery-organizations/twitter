{
  "info": {
    "name": "Twitter Show Members",
    "_postman_id": "48380477-5a7e-4117-a580-63b6cf49f63b",
    "description": "Check if the specified user is a member of the specified list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "9d8eef8a-806d-417d-86e6-14268d5daffc",
          "name": "check-if-the-specified-user-is-a-member-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members/show?include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check if the specified user is a member of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e97b4cd-515a-43b0-9b30-3b893da99c96"
            }
          ]
        }
      ]
    }
  ]
}