{
  "info": {
    "name": "Twitter User Lookup",
    "_postman_id": "984741f4-2fd8-4fd8-8269-0c783c2d6dd2",
    "description": "returns fully-hydrated user objects up to 100",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "23c80422-4915-41fd-b398-147aa2b52a7d",
          "name": "returns-fullyhydrated-user-objects-up-to-100",
          "request": {
            "url": "http://api.twitter.com/1.1/users/lookup?include_entities=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns fully-hydrated user objects up to 100"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57b50c1f-435f-4b3f-8e06-7cecc9886272"
            }
          ]
        }
      ]
    }
  ]
}