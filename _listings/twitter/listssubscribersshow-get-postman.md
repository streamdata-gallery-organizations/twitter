{
  "info": {
    "name": "Twitter Show List Subscribers",
    "_postman_id": "7ea30152-65a3-4ccd-a17a-64fffc465c06",
    "description": "Check if the specified user is a subscriber of the specified list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "de753709-7c44-4d46-b4c7-3aa0631ccb5c",
          "name": "check-if-the-specified-user-is-a-subscriber-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/show?include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check if the specified user is a subscriber of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b828eb8-9c01-4901-8382-2c957ff434a9"
            }
          ]
        }
      ]
    }
  ]
}