{
  "info": {
    "name": "Twitter Remove User From List",
    "_postman_id": "b6b7cfcb-93f3-4b90-bd0b-fe014951dc24",
    "description": "Returns the list of memebers destroy",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "00950297-1b59-4638-ba8b-2a9f223ae895",
          "name": "returns-the-list-of-memebers-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/members/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of memebers destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ba4070c-35bc-4d31-9513-bab776721489"
            }
          ]
        }
      ]
    }
  ]
}