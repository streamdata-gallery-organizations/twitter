{
  "info": {
    "name": "Twitter Update Profile Colors",
    "_postman_id": "a12000e1-cebb-4d98-ba60-ca21ed889eef",
    "description": "sets one or more hex values that controls color scheme",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Social",
      "item": [
        {
          "id": "418abe99-2729-459a-bbac-004576497387",
          "name": "returns-the-20-most-recent-mentions-for-the-authenticating-user",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/mentions_timeline?contributor_details=%7B%7D&count=%7B%7D&include_entities=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the 20 most recent mentions for the authenticating user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd660c6d-02c1-4548-982f-e02cea92bc90"
            }
          ]
        },
        {
          "id": "06116bdd-2e9d-4f6d-a815-ad063e03a096",
          "name": "returns-a-collection-of-the-most-recent-tweets-posted-by-the-user",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/user_timeline.json?contributor_details=%7B%7D&count=%7B%7D&exclude_replies=%7B%7D&include_rts=%7B%7D&max_id=%7B%7D&screen_name=screen_name&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of the most recent Tweets posted by the User"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f28146d0-7121-421c-a883-98897cf8c06a"
            }
          ]
        },
        {
          "id": "fc055954-53f7-4df7-bb83-bd0e57c350b7",
          "name": "returns-a-collection-of-the-most-recent-tweets",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/home_timeline?contributor_details=%7B%7D&exclude_replies=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&trim_user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a collection of the most recent Tweets"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "408f9423-0a19-441b-898e-5a63ac77917d"
            }
          ]
        },
        {
          "id": "67b98ef6-4d63-4ea7-a8ad-0715f30ffb2d",
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
              "id": "edbdc8e2-c74c-4055-9467-4ed54ff3a3ef"
            }
          ]
        },
        {
          "id": "52d1d34b-a417-4b81-ba59-baf9afb269dc",
          "name": "retruns-a-single-tweet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "statuses/show/:id"
              ],
              "query": [
                {
                  "key": "include_entities",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "include_my_retweet",
                  "value": "%7B%7D",
                  "disabled": false
                },
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retruns a single Tweet"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03d8bfbe-49f0-4d90-b204-2343abd9b87e"
            }
          ]
        },
        {
          "id": "b31f171c-c548-449f-abb1-f704d98bfbfd",
          "name": "destroys-the-status-specified-by-the-required-id-parameter",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.twitter.com",
              "path": [
                "1.1",
                "statuses/destroy/:id"
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
            "description": "Destroys the status specified by the required ID parameter"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4059176-9037-412f-85c0-29e0d10cfc49"
            }
          ]
        },
        {
          "id": "9b8808f7-620a-4cf2-99ea-02ce08e3d8b7",
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
              "id": "4762a446-c385-4951-8ed2-645ebfc1ecf2"
            }
          ]
        },
        {
          "id": "3328db16-0737-46d4-b5c3-d8742cc1edc3",
          "name": "returns-information-allowing-the-creation-of-an-embedded-representation",
          "request": {
            "url": "http://api.twitter.com/1.1/statuses/oembed?align=%7B%7D&hide_media=%7B%7D&hide_thread=%7B%7D&id=%7B%7D&lang=%7B%7D&maxwidth=%7B%7D&related=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information allowing the creation of an embedded representation"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93635a7d-71ed-46e2-8b8b-a661cdd94179"
            }
          ]
        },
        {
          "id": "0dd4288e-1a60-4e90-96d6-b5e2eee93080",
          "name": "return-all-lists-the-authenticating-or-specified-user-subscribes-to-including-their-own",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/list?screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return all lists the authenticating or specified user subscribes to, including their own."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27a7e0ae-1540-4301-9293-e03725b25bd7"
            }
          ]
        },
        {
          "id": "05a15a5a-a62b-450b-b9e4-f8639b894def",
          "name": "returns-a-timeline-of-tweets-authored-by-memebers-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/statuses.json?count=%7B%7D&include_entities=%7B%7D&include_rts=%7B%7D&list_id=%7B%7D&max_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&since_id=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a timeline of tweets authored by memebers of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "79a73c48-01d9-4bb0-bc2b-222601e5c6e2"
            }
          ]
        },
        {
          "id": "81dff174-7f8d-4421-a6b6-e875c6b001d1",
          "name": "returns-the-list-of-memebers-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/members/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of memebers destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59cb5bad-2039-4f28-a713-c5f17d320d25"
            }
          ]
        },
        {
          "id": "2d07b2c0-a7e6-48eb-9aed-a9bea59d8849",
          "name": "returns-the-lists-of-the-specified-user-has-been-added-to",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/memberships?cursor=%7B%7D&filter_to_owned_lists=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the lists of the specified user has been added to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f38a9472-4383-44fd-81e7-117df0d7004d"
            }
          ]
        },
        {
          "id": "c0eb44d5-7959-4936-96de-2741d646ae57",
          "name": "returns-the-subscribers-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers?cursor=%7B%7D&include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the subscribers of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbca0a76-4a54-430c-ba99-a8ad673b7850"
            }
          ]
        },
        {
          "id": "91141751-09af-4dd2-8ed6-ec238b811351",
          "name": "subscribes-the-authenticated-user-to-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/create?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Subscribes the authenticated user to the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dea9d25b-1152-46c7-a617-fa8ed2aa3d5c"
            }
          ]
        },
        {
          "id": "0cf8a9bf-503e-4350-9996-61f2af79b9d5",
          "name": "check-if-the-specified-user-is-a-subscriber-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/show?include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check if the specified user is a subscriber of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abc98f00-47c7-42c3-a413-d9943434c50d"
            }
          ]
        },
        {
          "id": "ef60dddc-b504-4292-8ed0-91dfc826c9c6",
          "name": "returns-list-of-subscribers-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscribers/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of subscribers destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6db12b0e-61df-4261-8b44-1ae586034c20"
            }
          ]
        },
        {
          "id": "c1cb7ad8-cd85-4628-865c-8930fcbcf98d",
          "name": "returns-lists-of-members-create-all",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/members/create_all?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of members create_all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "013360c4-4f40-4387-8d2f-5a31e662cb90"
            }
          ]
        },
        {
          "id": "075785fb-bf3f-4d15-8d10-776cd06c5130",
          "name": "check-if-the-specified-user-is-a-member-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members/show?include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Check if the specified user is a member of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bdf26e8-cb6b-4c3c-8b67-e5fe0c794aaf"
            }
          ]
        },
        {
          "id": "78c2c0e4-dd6a-421a-b415-51b1a8af8e34",
          "name": "returns-the-members-of-the-specified-list",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members?cursor=%7B%7D&include_entities=%7B%7D&list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&skip_status=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the members of the specified list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5de3d504-e508-4745-ab9b-b4176de12c4b"
            }
          ]
        },
        {
          "id": "fa8d32e7-1be8-46e3-8395-7a77f43043a5",
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
              "id": "922b71bc-d4e9-4f3a-9eb6-f221cc6bd455"
            }
          ]
        },
        {
          "id": "37668140-7ac8-4b56-a835-6a2848862d2c",
          "name": "returns-list-of-destroy",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/destroy?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of destroy"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03c2d545-4d0a-41db-a4a9-e280764e2acf"
            }
          ]
        },
        {
          "id": "b341a869-37e9-43f6-b565-afc86cb4d963",
          "name": "returns-lists-of-updates",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/update?description=%7B%7D&list_id=%7B%7D&mode=%7B%7D&name=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93141989-0e6f-4a07-b0f0-d54e88697e38"
            }
          ]
        },
        {
          "id": "bd2e8f4d-5901-4028-ae17-14a0144cc7e8",
          "name": "returns-list-of-create",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/create?description=%7B%7D&mode=%7B%7D&name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of create"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c3dbe09-70f4-4d63-b621-ad23fb0674cb"
            }
          ]
        },
        {
          "id": "8876f690-974b-4080-8622-b0d6d192d992",
          "name": "returns-list-of-show",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/show?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&slug=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of show"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f227f48-60ac-4351-afb8-dc15c1c11bf5"
            }
          ]
        },
        {
          "id": "18dcd936-7dfa-434b-82d6-4eb199d95ef3",
          "name": "returns-list-of-subscriptions",
          "request": {
            "url": "http://api.twitter.com/1.1/lists/subscriptions?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns list of subscriptions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "df8c499d-9172-45f7-8ab0-b60860a0d148"
            }
          ]
        },
        {
          "id": "0daf3e08-e27a-42d2-8ce6-681a911c046c",
          "name": "returns-lists-of-destroy-all",
          "request": {
            "url": "http://api.twitter.com/1.1/list/members/destroy_all?list_id=%7B%7D&owner_id=%7B%7D&owner_screen_name=%7B%7D&screen_name=%7B%7D&slug=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns lists of destroy all"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48e93aae-affb-4550-9de9-203156ea95f4"
            }
          ]
        },
        {
          "id": "70ab7682-68ed-47e4-a5e7-f1b532763e48",
          "name": "return-20-most-recent-direct-messages-sent",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/sent?count=%7B%7D&include_entities=%7B%7D&max_id=%7B%7D&page=%7B%7D&since_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "return 20 most recent direct messages sent"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abf661c3-8224-4a75-9de6-d5e72f01db2b"
            }
          ]
        },
        {
          "id": "d6b8bca3-6417-4457-a041-d830b3aad604",
          "name": "returns-a-single-direct-message-specified-by-an-id",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/show?id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a single direct message specified by an id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9ebfb13-f010-4b38-9271-be6619b5cb0c"
            }
          ]
        },
        {
          "id": "30a93df5-6c34-43d2-9936-af535f4ad0ca",
          "name": "returns-collection-of-relevant-tweets-matching-query",
          "request": {
            "url": "http://api.twitter.com/1.1/search/tweets.json?callback=%7B%7D&count=%7B%7D&geocode=%7B%7D&include_entities=%7B%7D&lang=%7B%7D&locale=%7B%7D&max_id=%7B%7D&q=%7B%7D&result_type=%7B%7D&since_id=%7B%7D&until=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns collection of relevant Tweets matching query"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61b2db11-e62e-44ae-8c46-1bfe31f0cf28"
            }
          ]
        },
        {
          "id": "f38cbf73-18f1-46cc-9d42-ce720942199b",
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
              "id": "13bc8d5a-f5a8-447b-a8a4-df4e35ac5b68"
            }
          ]
        },
        {
          "id": "73b403dc-7128-4a3e-b6d0-6ea2e9dd4481",
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
              "id": "ffa463b1-5e95-45f9-b424-6803fd9c22d7"
            }
          ]
        },
        {
          "id": "8fea28a1-c517-4643-af18-835e8dee91c9",
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
              "id": "ff98d654-ddb1-4b35-bdb0-09bb27670608"
            }
          ]
        },
        {
          "id": "80711ce2-9d6f-4747-8905-a65c5ba04c4c",
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
              "id": "6715dd14-8d5e-4c5a-9a4c-a7b0d2130b33"
            }
          ]
        },
        {
          "id": "6fa53f8d-8056-493e-bc41-2b782f8f01ac",
          "name": "return-20-most-recent-direct-messages-sent-to-user",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages?include_entities=%7B%7D&max_id=%7B%7D&since_id=%7B%7D&skip_status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "return 20 most recent direct messages sent to user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a6771f4c-fcc1-432c-b234-9ef7cd434f85"
            }
          ]
        },
        {
          "id": "b6e1a177-aaab-40a6-9f94-f7e0c5c005cf",
          "name": "destroys-direct-messages-specified-in-required-id",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/destroy?id=%7B%7D&include_entities=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "destroys direct messages specified in required ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9c95e69-e9f6-4932-a57f-5975f1d1798c"
            }
          ]
        },
        {
          "id": "eaf00ac3-96df-4c2b-b271-2bfd960c8613",
          "name": "sends-a-new-direct-message-to-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/direct_messages/new?screen_name=%7B%7D&text=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sends a new direct message to specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1cfd961d-9d75-4681-b015-82610e22bad6"
            }
          ]
        },
        {
          "id": "db0a2f02-5faf-4a07-9d3a-e84b0fe705d6",
          "name": "returns-a-cursored-collection-of-user-ids-followed-by-user",
          "request": {
            "url": "http://api.twitter.com/1.1/friends/ids?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&stringify_ids=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a cursored collection of user IDs followed by user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c40a39ff-fda2-4e48-97fe-5bcfa13a71f2"
            }
          ]
        },
        {
          "id": "9bcf1803-9eb3-4cf3-b9b9-f06b082b2e97",
          "name": "returns-a-cursored-collection-of-user-ids-following-the-user",
          "request": {
            "url": "http://api.twitter.com/1.1/followers/ids?count=%7B%7D&cursor=%7B%7D&screen_name=%7B%7D&stringify_ids=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a cursored collection of user IDs following the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4079a1e1-f0f1-47ea-81e1-466e20742f67"
            }
          ]
        },
        {
          "id": "c54ead53-b379-431e-af61-66ea64ecfa79",
          "name": "returns-collection-of-ids-of-users-with-pending-follow-request",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/incoming?cursor=%7B%7D&stringify_ids=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns collection of IDs of users with pending follow request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2040de3e-058c-4e08-8cd5-a06aa6e5306d"
            }
          ]
        },
        {
          "id": "19e1347d-8b66-43c6-b91d-791dd8ef4d36",
          "name": "returns-collection-of-ids-of-users-with-pending-follow-request-from-the-user",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/outgoing?cursor=%7B%7D&stringify_ids=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns collection of IDs of users with pending follow request from the user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf5c7f7d-e915-4375-ac94-ddf71edffdf1"
            }
          ]
        },
        {
          "id": "ccb044a1-4b06-46f0-a2ff-b4b153ce0200",
          "name": "allows-users-to-follow-user-sepcified-by-id",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/create?follow=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "allows users to follow user sepcified by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6332f37c-d7dc-48bc-bb36-3f7f6c55df9d"
            }
          ]
        },
        {
          "id": "a654d1f5-022d-4edf-a8d4-699fc54f9bb7",
          "name": "allows-user-to-unfollow-user-psecified-by-id",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/destroy?screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "allows user to unfollow user psecified by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e6def6e-26da-467f-a43e-76906eb7ed6e"
            }
          ]
        },
        {
          "id": "9b52cdad-7e4b-490e-978e-938ee53d25ac",
          "name": "allows-one-to-enable-or-disable-settings-for-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/update?device=%7B%7D&retweets=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Allows one to enable or disable settings for specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b4b189d-b102-43c6-8462-6bd9d59dfafb"
            }
          ]
        },
        {
          "id": "66962fa3-af63-460e-b6c1-7c1bae9f07f7",
          "name": "returns-detailed-info-about-relationship-between-two-users",
          "request": {
            "url": "http://api.twitter.com/1.1/friendships/show?source_id=%7B%7D&source_screen_name=%7B%7D&target_id=%7B%7D&target_screen_name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns detailed info about relationship between two users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e4142e5-9aa9-4700-aa07-2b0e87491858"
            }
          ]
        },
        {
          "id": "2817f5cb-5359-4e66-a9da-b8aacc120ab2",
          "name": "returns-settings-for-user",
          "request": {
            "url": "http://api.twitter.com/1.1/account/settings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns settings for user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b2a1207-dce3-4671-8149-42951b9ba7c6"
            }
          ]
        },
        {
          "id": "5938a900-19b6-49df-9c4e-3548aae4ecea",
          "name": "updates-users-settings",
          "request": {
            "url": "http://api.twitter.com/1.1/account/settings?end_sleep_time=%7B%7D&lang=%7B%7D&sleep_time_enabled=%7B%7D&start_sleep_time=%7B%7D&time_zone=%7B%7D&trend_location_woeid=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "updates user's settings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "025c5e21-d26a-46bf-b1fd-bd58dc6f72d8"
            }
          ]
        },
        {
          "id": "d488a31e-fd6c-4c2a-b44c-b2904cf6297a",
          "name": "sets-which-device-twitter-delivers-updates-to-for-user",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_delivery_device?device=%7B%7D&include_entities=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sets which device Twitter delivers updates to for user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0067c814-dd1e-40cf-8dd2-2421babfea0f"
            }
          ]
        },
        {
          "id": "88f48179-8b13-42a7-85ab-8300c2f070c7",
          "name": "sets-values-that-users-ar-eable-to-set-under-account-tab",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_profile?description=%7B%7D&include_entities=%7B%7D&location=%7B%7D&name=%7B%7D&skip_status=%7B%7D&url=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sets values that users ar eable to set under Account tab"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af0c986b-7382-402c-8b30-231c6b5fae88"
            }
          ]
        },
        {
          "id": "f5e5098c-3f0c-4fd1-a06e-f6b8a8b5ea8e",
          "name": "updates-users-profile-background-image",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_profile_background_image?include_entities=%7B%7D&skip_status=%7B%7D&tile=%7B%7D&use=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "file",
                  "value": "{}",
                  "disabled": false,
                  "description": "image to replace background image of profile"
                }
              ]
            },
            "description": "updates user's profile background image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "661df9dd-d6d6-464d-af9a-a2bbf765b6c8"
            }
          ]
        },
        {
          "id": "d1a8cd2a-23e9-4058-b2ea-b4c5ce8613e0",
          "name": "sets-one-or-more-hex-values-that-controls-color-scheme",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_profile_colors?include_entities=%7B%7D&profile_background_color=%7B%7D&profile_link_color=%7B%7D&profile_sidebar_border_color=%7B%7D&profile_sidebar_fill_color=%7B%7D&profile_text_color=%7B%7D&skip_status=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "sets one or more hex values that controls color scheme"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47d2d55a-6cfc-4a45-907c-b76ba6b2cde3"
            }
          ]
        }
      ]
    }
  ]
}