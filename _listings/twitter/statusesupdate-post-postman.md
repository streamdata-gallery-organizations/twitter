{
  "info": {
    "name": "Twitter Update Status",
    "_postman_id": "85b56f08-18a6-447d-aef9-e0b314a38803",
    "description": "Updates the authenticating user's status",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "4e011991-799c-480d-ac06-1f52d79aeb93",
          "name": "updates-the-authenticating-users-status",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/update?display_coordinates=%7B%7D&in_reply_to_status_id=%7B%7D&lat=%7B%7D&long=%7B%7D&place_id=%7B%7D&status=%7B%7D&trim_user=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the authenticating user's status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "682e09d4-325d-485d-a149-560e9c05c038"
            }
          ]
        }
      ]
    }
  ]
}