{
  "info": {
    "name": "Twitter Get Memberships",
    "_postman_id": "6c5e2f3d-9b54-4024-8dcc-099979fe3ba9",
    "description": "Returns the lists of the specified user has been added to",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "f32119b0-caf5-408a-b3a4-954e70b172f0",
          "name": "returns-the-lists-of-the-specified-user-has-been-added-to",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/memberships?cursor=%7B%7D&filter_to_owned_lists=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the lists of the specified user has been added to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbe5ff89-a39d-4ced-8e7f-0fa2b8bff08e"
            }
          ]
        }
      ]
    }
  ]
}