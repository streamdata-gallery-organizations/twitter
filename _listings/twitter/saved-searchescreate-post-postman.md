{
  "info": {
    "name": "Twitter Create Saved Search",
    "_postman_id": "a397af6c-2324-4790-bb90-90d38feae349",
    "description": "Create a new saved search for the authenticated user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "eecabd03-c998-49d4-a74e-5f6cbb463677",
          "name": "create-a-new-saved-search-for-the-authenticated-user",
          "request": {
            "url": "http://api.twitter.com/1.1/saved_searches/create?query=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new saved search for the authenticated user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9d03131-8d58-48ff-9a3e-3658ac8f32d4"
            }
          ]
        }
      ]
    }
  ]
}