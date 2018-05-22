{
  "info": {
    "name": "Twitter Get Lat / Log",
    "_postman_id": "06a7a727-f7e3-4d66-a5e5-cb603dcea4a4",
    "description": "Given a latitude and a longitude, searches for up to 20 places that can be used as a place_id when updatting a status",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "places",
      "item": [
        {
          "id": "06e07c85-2341-4d04-a7d6-fd3ba0470dc2",
          "name": "given-a-latitude-and-a-longitude-searches-for-up-to-20-places-that-can-be-used-as-a-place-id-when-up",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/reverse_geoncode?accuracy=%7B%7D&callback=%7B%7D&granularity=%7B%7D&lat=%7B%7D&long=%7B%7D&max_results=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a latitude and a longitude, searches for up to 20 places that can be used as a place_id when updatting a status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "199e3542-2e01-482c-871f-27ea2a937942"
            }
          ]
        }
      ]
    }
  ]
}