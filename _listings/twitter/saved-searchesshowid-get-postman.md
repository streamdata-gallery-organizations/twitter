{
  "info": {
    "name": "Twitter Get Saved Search",
    "_postman_id": "bb5a1f77-68ed-4d7f-bdd8-0b0bf0e7ff72",
    "description": "Retrieve the information for the saved search represented by the given id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "bf859352-e5c4-4cbc-a026-b5e48e517b70",
          "name": "retrieve-the-information-for-the-saved-search-represented-by-the-given-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "saved_searches/show/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the information for the saved search represented by the given id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c2e2a35-3653-49a6-b50c-6d9aa25d25cc"
            }
          ]
        }
      ]
    }
  ]
}