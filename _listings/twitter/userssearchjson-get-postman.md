{
  "info": {
    "name": "Twitter User Search",
    "_postman_id": "d4d009cd-3b1f-4bea-bcbd-05c593261b96",
    "description": "simple relevance-based user search",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "148c9dc2-67ad-4bbe-8e1b-021e8a4ad533",
          "name": "simple-relevancebased-user-search",
          "request": {
            "url": "http://api.twitter.com/1.1/users/search.json?count=%7B%7D&include_entities=%7B%7D&page=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "simple relevance-based user search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf295016-3832-454b-9483-5732320dde5a"
            }
          ]
        }
      ]
    }
  ]
}