{
  "info": {
    "name": "Twitter Show Available Trends",
    "_postman_id": "ac7bcca6-0195-49f8-886d-3279d9531e8c",
    "description": "Returns the availability",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "24186e4e-c615-4174-910c-2425139235d9",
          "name": "returns-the-availability",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/available.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the availability"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db6930af-cfdb-45b6-8e6c-52ce959a5181"
            }
          ]
        }
      ]
    }
  ]
}