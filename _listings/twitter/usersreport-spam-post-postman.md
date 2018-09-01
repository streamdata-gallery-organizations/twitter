{
  "info": {
    "name": "Twitter Report User Spam",
    "_postman_id": "dd481840-385a-4546-8bb9-222ba60e508b",
    "description": "Returna users report spam",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "4a814650-e95f-4af7-9ef6-69794e25d450",
          "name": "returna-users-report-spam",
          "request": {
            "url": "http://api.twitter.com/1.1/users/report_spam?screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returna users report spam"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a7d329a-266e-4081-911b-64714761fa36"
            }
          ]
        }
      ]
    }
  ]
}