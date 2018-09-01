{
  "info": {
    "name": "Twitter Remove Direct Message",
    "_postman_id": "e9efb9f3-91b5-44d0-978a-b2daa3ef170d",
    "description": "destroys direct messages specified in required ID",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "64fc6a3a-382c-4af2-86f4-8a794df0d64f",
          "name": "destroys-direct-messages-specified-in-required-id",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/destroy?id=%7B%7D&include_entities=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "destroys direct messages specified in required ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e2212f9-7eb0-4c2a-b79e-a4f5a669c9a9"
            }
          ]
        }
      ]
    }
  ]
}