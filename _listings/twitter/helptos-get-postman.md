{
  "info": {
    "name": "Twitter Help Terms of Services",
    "_postman_id": "1a24cbea-1875-4abe-8d65-addd66f2e935",
    "description": "Returns the Twitter Terms of Service",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "99c42591-668b-488c-be9a-d8f3532bf518",
          "name": "returns-the-twitter-terms-of-service",
          "request": {
            "url": "http://api.twitter.com/1.1/help/tos",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the Twitter Terms of Service"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edf392e6-0f8d-4c00-9705-5837173241e3"
            }
          ]
        }
      ]
    }
  ]
}