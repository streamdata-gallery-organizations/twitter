{
  "info": {
    "name": "Twitter Get Place",
    "_postman_id": "fd648dd6-603d-4b07-a450-4dc8084eb299",
    "description": "Returns all the information about a know place",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "places",
      "item": [
        {
          "id": "8422e678-fae1-4c98-b5e4-a3f019ddf320",
          "name": "returns-all-the-information-about-a-know-place",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "geo/id/:place_id"
              ],
              "variable": [
                {
                  "id": "place_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all the information about a know place"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3328e78e-3e8d-444b-bd3d-bfb4d0d0f27d"
            }
          ]
        }
      ]
    }
  ]
}