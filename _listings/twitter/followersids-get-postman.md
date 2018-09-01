{
  "info": {
    "name": "Twitter Get Followers",
    "_postman_id": "7aba26d5-15ab-4718-b34e-c5291df45e75",
    "description": "returns a cursored collection of user IDs following the user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Social",
      "item": [
        {
          "id": "037c209c-eb2a-4ff3-acfd-54da2c485b49",
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
              "id": "84ee49d8-1049-4361-ba60-e11d166ef467"
            }
          ]
        },
        {
          "id": "9390cf0a-5dc6-4839-9187-7dcabf4ad892",
          "name": "returns-a-cursored-collection-of-user-ids-following-the-user",
          "request": {
            "url": "http://api.twitter.com/1.1/followers/ids?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&stringify_ids=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a cursored collection of user IDs following the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87c93d93-a850-45c8-b7e9-311767465c07"
            }
          ]
        }
      ]
    }
  ]
}