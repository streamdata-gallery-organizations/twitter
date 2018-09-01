{
  "info": {
    "name": "Twitter List Subscribers",
    "_postman_id": "ffa9c19f-70f0-4d33-b16a-d811766ae91a",
    "description": "Returns the subscribers of the specified list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "be7bbe02-bee3-4108-9239-2efc40a2ae4a",
          "name": "returns-the-subscribers-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers?cursor=%7B%7D&include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the subscribers of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50885b5e-b5f1-4c2b-8f85-0b6dec16fb68"
            }
          ]
        }
      ]
    }
  ]
}