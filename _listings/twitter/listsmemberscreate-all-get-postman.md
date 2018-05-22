{
  "info": {
    "name": "Twitter Add Users to List",
    "_postman_id": "523bd7c0-d2ba-432f-aacd-5ad1776aac9c",
    "description": "Returns lists of members create_all",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "dfd4b249-16a6-4988-a288-bfa29ce62096",
          "name": "returns-lists-of-members-create-all",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/members/create_all?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of members create_all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fb38920-a85a-4e6c-84d0-ff45d9754277"
            }
          ]
        }
      ]
    }
  ]
}