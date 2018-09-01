{
  "info": {
    "name": "Twitter User Contributees",
    "_postman_id": "b6395ce7-5bfb-4b28-bb99-86a81332e824",
    "description": "collection of users specified user can contribute to",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "db706a04-a65e-4de6-b5b7-31a8491629a3",
          "name": "collection-of-users-specified-user-can-contribute-to",
          "request": {
            "url": "http://api.twitter.com/1.1/users/contributees?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "collection of users specified user can contribute to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ecc7a88f-3dfc-4386-8a69-255de4263e8a"
            }
          ]
        }
      ]
    }
  ]
}