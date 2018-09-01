{
  "info": {
    "name": "Twitter Get Places",
    "_postman_id": "9dc2890f-27aa-422e-9c13-b70a8e4307a7",
    "description": "Create a new place object at the given latitude and logitude",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "places",
      "item": [
        {
          "id": "59a65e14-6ea4-48b0-8a5a-33b0b3b7e299",
          "name": "create-a-new-place-object-at-the-given-latitude-and-logitude",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/places?attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&lat=%7B%7D&long=%7B%7D&name=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new place object at the given latitude and logitude"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aba80c1e-9b5a-4bbd-bad9-78667e517ba8"
            }
          ]
        }
      ]
    }
  ]
}