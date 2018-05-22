{
  "info": {
    "name": "Twitter Show LIsts",
    "_postman_id": "39fb32e5-5440-400d-8f5b-224fb027c8b4",
    "description": "Returns list of show",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "3d497f5e-a5a9-45ab-b77f-f5fff31ce740",
          "name": "returns-list-of-show",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/show?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of show"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1ac360f-04d8-4847-81bb-c637bb210480"
            }
          ]
        }
      ]
    }
  ]
}