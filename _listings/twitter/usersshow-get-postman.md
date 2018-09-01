{
  "info": {
    "name": "Twitter Show User",
    "_postman_id": "e84395bb-8fdb-4ae9-9ecb-9f5781f5540c",
    "description": "returns a variety of info about specified user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "53f06473-982f-47cd-b639-57a90031e47c",
          "name": "returns-a-variety-of-info-about-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/users/show?include_entities=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a variety of info about specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40caa8c8-0b36-4103-b409-4cf5de396876"
            }
          ]
        }
      ]
    }
  ]
}