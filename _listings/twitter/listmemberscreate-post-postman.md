{
  "info": {
    "name": "Twitter Add Member",
    "_postman_id": "c8e337ec-65be-42a3-9501-132cc54b2ac4",
    "description": "Returns list of members create",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "1ab00f2b-5160-4e26-b451-3726472783f6",
          "name": "returns-list-of-members-create",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members/create?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of members create"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4689b12-07de-4b05-afe8-e53306b8bb95"
            }
          ]
        }
      ]
    }
  ]
}