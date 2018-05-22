{
  "info": {
    "name": "Twitter Help Langues",
    "_postman_id": "9f7e42b0-e8a3-4550-8327-b53b8cf7bd3f",
    "description": "Returns the list of languages supported by Twitter along with the language code supported by Twitter",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "languages",
      "item": [
        {
          "id": "658545d6-43e9-4b24-ae8b-b43850fdf9c0",
          "name": "returns-the-list-of-languages-supported-by-twitter-along-with-the-language-code-supported-by-twitter",
          "request": {
            "url": "http://api.twitter.com/1.1/help/languages",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of languages supported by Twitter along with the language code supported by Twitter"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e011c8d3-5cb3-4081-9fcb-020ee90ff8f4"
            }
          ]
        }
      ]
    }
  ]
}