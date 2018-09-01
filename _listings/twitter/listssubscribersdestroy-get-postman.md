{
  "info": {
    "name": "Twitter Remove List Subscribers",
    "_postman_id": "38a031ee-552a-414d-b5ff-ac303b4adc61",
    "description": "Returns list of subscribers destroy",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "0073915b-5780-490b-88b2-784b48decd41",
          "name": "returns-list-of-subscribers-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of subscribers destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83dc2ae5-565b-438a-baf3-c51bd29138d7"
            }
          ]
        }
      ]
    }
  ]
}