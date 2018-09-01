{
  "info": {
    "name": "Twitter Show Retweets",
    "_postman_id": "ad58e649-f412-4548-b63e-1370c97cd8ef",
    "description": "Retweens a tweet",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "social",
      "item": [
        {
          "id": "6507635a-a1a5-402b-b1a9-486f866bb8c5",
          "name": "retweens-a-tweet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "statuses/retweets/:id"
              ],
              "query": [
                {
                  "key": "trim_user",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Retweens a tweet"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af2304d4-f2dd-4698-8b1f-e23c6f915e37"
            }
          ]
        }
      ]
    }
  ]
}