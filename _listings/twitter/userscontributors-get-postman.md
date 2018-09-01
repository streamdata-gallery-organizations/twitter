{
  "info": {
    "name": "Twitter User Contributors",
    "_postman_id": "936a0059-5dff-4ae6-88ee-1b286cf6ecd0",
    "description": "collection of users that can contribute to specified account",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "ab767210-d63f-4bec-972a-43cccb9db5fb",
          "name": "collection-of-users-that-can-contribute-to-specified-account",
          "request": {
            "url": "http://api.twitter.com/1.1/users/contributors?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "collection of users that can contribute to specified account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c954d372-7ea3-4c0e-8e6d-698145f62153"
            }
          ]
        }
      ]
    }
  ]
}