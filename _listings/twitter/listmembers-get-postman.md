{
  "info": {
    "name": "Twitter Get Members",
    "_postman_id": "d43d9b9f-1cf1-477d-8d87-698f807c03d1",
    "description": "Returns the members of the specified list",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "a81774d8-8eb3-4b1e-b2b9-80b09ff2a212",
          "name": "returns-the-members-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members?cursor=%7B%7D&include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the members of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4db74d8c-c9f9-400e-ae8c-9aff67f6051a"
            }
          ]
        }
      ]
    }
  ]
}