{
  "info": {
    "name": "Twitter Help Privacy",
    "_postman_id": "26bc5cb5-65e8-4bd7-8b81-559ade227776",
    "description": "Returns Twitter's privacy policy",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "terms of service",
      "item": [
        {
          "id": "9ae5e877-a5c3-4ad0-addd-36e9a43b3e14",
          "name": "returns-twitters-privacy-policy",
          "request": {
            "url": "http://api.twitter.com/1.1/help/privacy",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns Twitter's privacy policy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64ec6881-ce10-44d5-8b7a-497085e75cbd"
            }
          ]
        }
      ]
    }
  ]
}