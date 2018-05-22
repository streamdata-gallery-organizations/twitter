{
  "info": {
    "name": "Twitter Create List",
    "_postman_id": "5ed4bdfa-0faa-4ac1-b536-930a71f0527a",
    "description": "Returns list of create",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "ae02f9cf-0e15-47b3-9e22-5e480f3a4716",
          "name": "returns-list-of-create",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/create?description=%7B%7D&mode=%7B%7D&name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of create"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "84721b60-4c30-4e16-b692-b0fc17bcea93"
            }
          ]
        }
      ]
    }
  ]
}