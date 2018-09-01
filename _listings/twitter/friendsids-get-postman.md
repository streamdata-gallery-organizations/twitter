{
  "info": {
    "name": "Twitter Get Friends",
    "_postman_id": "f260afe3-0a7f-4fe9-a00b-f08e42e1e5ff",
    "description": "returns a cursored collection of user IDs followed by user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Social",
      "item": [
        {
          "id": "1e38f863-2b66-4aa4-8278-7742b8f02050",
          "name": "returns-a-cursored-collection-of-user-ids-followed-by-user",
          "request": {
            "url": "http://api.twitter.com/1.1/friends/ids?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&stringify_ids=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a cursored collection of user IDs followed by user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af89e5db-8977-4f10-b2d7-06001bbfdd16"
            }
          ]
        }
      ]
    }
  ]
}