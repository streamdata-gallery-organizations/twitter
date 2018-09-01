{
  "info": {
    "name": "Twitter Remove Members",
    "_postman_id": "53b3ef58-1061-4c93-9890-0a0ad290fea5",
    "description": "Returns lists of destroy all",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "634cee4f-b7a4-4c89-adca-02c3e22f0e8d",
          "name": "returns-lists-of-destroy-all",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members/destroy_all?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of destroy all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7c1cd6d-3a07-44d9-bb5e-6937fd6fa962"
            }
          ]
        }
      ]
    }
  ]
}