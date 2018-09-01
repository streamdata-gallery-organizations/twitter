{
  "info": {
    "name": "Twitter List LIst",
    "_postman_id": "44515ccf-24fe-44f9-ad03-f4b3cfb42bda",
    "description": "Return all lists the authenticating or specified user subscribes to, including their own.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "9d7c8af6-00ce-4e65-ac26-9d04724a363c",
          "name": "return-all-lists-the-authenticating-or-specified-user-subscribes-to-including-their-own",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/list?screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return all lists the authenticating or specified user subscribes to, including their own"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a937c20-4cf7-4067-b505-287bcb2e8b2f"
            }
          ]
        }
      ]
    }
  ]
}