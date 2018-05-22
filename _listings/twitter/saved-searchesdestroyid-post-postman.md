{
  "info": {
    "name": "Twitter Destroy Saved Search",
    "_postman_id": "b92c71c8-aed3-434b-a9b9-a598f7cde605",
    "description": "Destroy a saved search for the authenticating user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "5f438435-60f9-4b6d-b577-18abb5354e8f",
          "name": "destroy-a-saved-search-for-the-authenticating-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "saved_searches/destroy/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Destroy a saved search for the authenticating user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "57ea83df-fd81-4ea0-93af-2bc8b24bc7be"
            }
          ]
        }
      ]
    }
  ]
}