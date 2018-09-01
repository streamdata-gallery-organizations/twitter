{
  "info": {
    "name": "Twitter List Saved Searches",
    "_postman_id": "8c44403e-b043-4815-abe4-5c0b55f69e15",
    "description": "Returns the authenticated user's saved search queries",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "0c678f98-0f47-409a-a757-c341a675d877",
          "name": "returns-the-authenticated-users-saved-search-queries",
          "request": {
            "url": "http://api.twitter.com/1.1/saved_searches/list",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated user's saved search queries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ebe63fb-ace9-40e3-b40a-fb8f4c7efce3"
            }
          ]
        }
      ]
    }
  ]
}