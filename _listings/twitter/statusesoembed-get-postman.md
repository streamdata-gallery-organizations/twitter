{
  "info": {
    "name": "Twitter Oembed Statuses",
    "_postman_id": "3fd940fe-9d5f-4111-98c8-1448d3ea1342",
    "description": "Returns information allowing the creation of an embedded representation",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "1957baaf-6782-406a-89af-2c01e4dd7a53",
          "name": "returns-information-allowing-the-creation-of-an-embedded-representation",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/oembed?align=%7B%7D&hide_media=%7B%7D&hide_thread=%7B%7D&id=%7B%7D&lang=%7B%7D&maxwidth=%7B%7D&related=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information allowing the creation of an embedded representation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fbb02a2-d173-443a-94b1-d0456e471383"
            }
          ]
        }
      ]
    }
  ]
}