{
  "info": {
    "name": "Twitter Get Friend Requests",
    "_postman_id": "36254cf9-7c9d-49f0-9fd0-4b5c259b3845",
    "description": "returns collection of IDs of users with pending follow request",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Social",
      "item": [
        {
          "id": "fc7007e4-c58a-4c3e-a6dc-ae8da94b9a84",
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
              "id": "12802657-1b42-4d7f-a8de-bbe14a2b19b4"
            }
          ]
        },
        {
          "id": "94a11236-350b-4c91-bd40-67a654f0aa7e",
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
              "id": "59959304-0ae0-4b3c-b4c1-ce94f4a26e41"
            }
          ]
        },
        {
          "id": "0cbbf59f-5b47-4ef4-a84c-05960c6b3ec7",
          "name": "returns-collection-of-ids-of-users-with-pending-follow-request",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/incoming?cursor=%7B%7D&stringify_ids=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns collection of IDs of users with pending follow request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbc42f41-db0b-4b7a-9e5e-1c2ebda99f7c"
            }
          ]
        }
      ]
    }
  ]
}