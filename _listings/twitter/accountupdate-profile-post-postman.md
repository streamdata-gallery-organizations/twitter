{
  "info": {
    "name": "Twitter Update Profile",
    "_postman_id": "787da888-d310-4015-94d1-8b75a24a8246",
    "description": "sets values that users ar eable to set under Account tab",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Social",
      "item": [
        {
          "id": "5c970ebb-9776-4900-8199-de0d702890b1",
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
              "id": "ee4e894f-ca4a-4a5d-8ddd-a65a123213dc"
            }
          ]
        },
        {
          "id": "d6c416a8-4855-4df6-bb75-7d53c6b90ea0",
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
              "id": "1ec29288-1754-4add-917c-539df73e40ed"
            }
          ]
        },
        {
          "id": "a4c1264d-a8fa-4276-a14e-30c96eef050a",
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
              "id": "d89f7d8b-2316-4755-802a-4f253b68555e"
            }
          ]
        },
        {
          "id": "47af1bfc-91ef-4890-89aa-29b3f4b2bce4",
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
              "id": "4161e7aa-4c9a-4ba0-8952-35f3fcc0163e"
            }
          ]
        },
        {
          "id": "0b628178-ba9b-4c45-ab30-d18a487b91d0",
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
              "id": "86b2b8ed-5247-4889-abda-ab2b1179c88a"
            }
          ]
        },
        {
          "id": "58a2420c-c206-42ba-95cd-a2fe233e789b",
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
              "id": "f58a0fa1-6838-4b56-af12-40bdd18846c8"
            }
          ]
        },
        {
          "id": "3cbee1aa-a07a-4e06-aa8a-4f086d9bcc35",
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
              "id": "57e1c57a-0d02-48e2-a28d-fda8b083d0f4"
            }
          ]
        },
        {
          "id": "b4a0b7e8-bef9-452e-9ac7-701351c8a237",
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
              "id": "1996556f-8e2b-4ae7-8eb2-da2847f74d39"
            }
          ]
        },
        {
          "id": "04e48ffc-570d-4db5-8214-269fcccc8efe",
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
              "id": "3d61a359-8a38-4458-8f8f-b5a669471385"
            }
          ]
        },
        {
          "id": "0ebc211d-3a87-4d15-8bff-c0d7ef7869f6",
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
              "id": "f7d6f92a-ab11-45df-8259-10d7f0e935e9"
            }
          ]
        },
        {
          "id": "b0e6f462-78f5-489c-a8ee-6992ff96bc6d",
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
              "id": "e9272ca0-80bb-4d75-bcd9-027ef94c7d49"
            }
          ]
        },
        {
          "id": "1274bc44-8317-432e-be8b-1ee88ffe6d19",
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
              "id": "8e2b0328-51cf-4313-93c8-e7bb63dbfbaf"
            }
          ]
        },
        {
          "id": "9bb824ca-a050-4e5f-a751-c79c9b72de83",
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
              "id": "b19f2843-fdb3-4905-a117-ec6d4f96685d"
            }
          ]
        },
        {
          "id": "29bab7f1-a970-40c8-94fd-cf9c4fa44aef",
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
              "id": "63adf0dc-4578-43e6-af76-60f2b52ff5bd"
            }
          ]
        },
        {
          "id": "81b2aeb4-cbc1-4b31-a22a-6f5909184b09",
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
              "id": "091c00c2-1bae-4209-8e71-ba46ce64ee06"
            }
          ]
        },
        {
          "id": "04fdfc38-3c48-4b28-b253-13e87ff783de",
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
              "id": "e2fbac96-7df7-4d82-897a-061908c40ff2"
            }
          ]
        },
        {
          "id": "8c4fe228-8d8c-471e-9a99-ffc850dd5c20",
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
              "id": "6294d710-d119-48ad-b428-27cff839c29a"
            }
          ]
        },
        {
          "id": "5cc8c9b6-5bba-474f-bd38-d70e71a4a0a0",
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
              "id": "31bbe5ed-b790-4d87-adb6-a40de8a383ce"
            }
          ]
        },
        {
          "id": "b7b6ac84-f04c-45ed-bfa6-55d1b3712ffb",
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
              "id": "49f9e628-0692-4325-9f2c-d1b9734e1306"
            }
          ]
        },
        {
          "id": "646379a6-83c4-46d3-98c2-a97a60b624fc",
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
              "id": "bde336a3-8748-4aea-993e-f234435ed270"
            }
          ]
        },
        {
          "id": "6c95cfcd-7b2d-409d-a510-ec286377b558",
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
              "id": "9aec80a7-3d7d-4123-87b7-8574707752ad"
            }
          ]
        },
        {
          "id": "60ce9465-9e38-4eea-9a7c-3c6f0220e386",
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
              "id": "6077497b-e892-4248-aae7-7b84ba94d646"
            }
          ]
        },
        {
          "id": "b7226ad8-3d21-4d73-8c65-9038133c8ce8",
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
              "id": "516d9246-ca56-40e5-8e1b-bc1c43eab3fe"
            }
          ]
        },
        {
          "id": "316867da-928d-4464-8422-b151f056cb82",
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
              "id": "ec44c981-3b59-4041-84f0-3d831bf0cfaa"
            }
          ]
        },
        {
          "id": "4b45246f-98cf-4458-a4ae-f1be80301b7d",
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
              "id": "86e77a20-9415-4dce-bada-7bc0de151ef1"
            }
          ]
        },
        {
          "id": "af710233-76be-43f2-8c86-5f681832d676",
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
              "id": "ba884019-0f03-4865-a61c-20e7bb8fa37c"
            }
          ]
        },
        {
          "id": "79a5358b-f48d-4b74-a98b-350f299ed25f",
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
              "id": "78fa8b48-2ee5-44cd-9357-ecd17e2840b7"
            }
          ]
        },
        {
          "id": "e5dc38e3-b7a6-4a93-965e-611f3f54c4fb",
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
              "id": "8a2ebffb-5721-468d-887e-621bc390f19b"
            }
          ]
        },
        {
          "id": "8ac11238-12fb-4f4d-8d1c-a14705fa66a4",
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
              "id": "8beb0ced-a4a9-4788-9aae-c11d8f8e9904"
            }
          ]
        },
        {
          "id": "2234ca23-8544-4f7b-8559-b86ef51f28cc",
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
              "id": "5b54e162-479c-4a6a-bbcf-f7ba6fd05570"
            }
          ]
        },
        {
          "id": "3516d5bf-0f1e-489a-a6f9-068477b21f4b",
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
              "id": "810262fd-09c4-4f61-920f-e18d011b44db"
            }
          ]
        },
        {
          "id": "67d6e873-96db-4656-94cd-16f8993c0fcc",
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
              "id": "1c386e39-6da5-45fc-b688-e0fa821ff190"
            }
          ]
        },
        {
          "id": "5553fe57-a550-4a72-a579-8321d5e587bb",
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
              "id": "c8e78a53-dd2a-4a38-900d-280bf350c3a3"
            }
          ]
        },
        {
          "id": "8649d674-6b85-49db-87e4-33fc1a13a2ed",
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
              "id": "0b72a125-d3ab-4ba1-9675-f97dc299e5d0"
            }
          ]
        },
        {
          "id": "49fb8266-90eb-40bc-9326-e44f84ea3657",
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
              "id": "c5510cae-9aa2-4e60-9d35-76e1bdc1b379"
            }
          ]
        },
        {
          "id": "dba1692e-85b5-458f-9b2f-3e7f9bbf8fcd",
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
              "id": "54c738ba-c724-48d1-a5b3-eb48561ff024"
            }
          ]
        },
        {
          "id": "112967c3-f9dd-45cc-a21b-9e240b0c82bf",
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
              "id": "64f50cbb-1776-462e-9edf-2261a6bf21c5"
            }
          ]
        },
        {
          "id": "259d86c3-c15c-45ea-b5b4-6406fc0081a5",
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
              "id": "fdfdf90a-9a2e-4ddc-a02d-ffe2ad3b5e88"
            }
          ]
        },
        {
          "id": "361a5690-a3ed-4d9e-a138-1f2872c4cee6",
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
              "id": "98c6c2a8-204f-44e7-80bc-983a9f9e3a25"
            }
          ]
        },
        {
          "id": "44440d28-0ad9-40be-aa01-44447c31404b",
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
              "id": "a850d6ac-5c8c-4e23-89b4-0ec7de788665"
            }
          ]
        },
        {
          "id": "c364aa85-d036-4434-b8a4-e0b4547757d7",
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
              "id": "6b0099ed-aeb5-44d2-9175-c4ba46a8d314"
            }
          ]
        },
        {
          "id": "c472cc38-3e74-4fed-975b-5d828bddad25",
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
              "id": "05c6b638-862f-49d6-a86e-683b08cb7975"
            }
          ]
        },
        {
          "id": "aee7070b-df38-4aff-be82-b5762c51060c",
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
              "id": "f0e3c7cd-a3f4-4834-b757-17a36a48a730"
            }
          ]
        },
        {
          "id": "51c80d1a-17d3-4de1-84ad-6608fc36bc4e",
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
              "id": "86fc568e-b7dc-45a8-8481-0ec189da6a04"
            }
          ]
        },
        {
          "id": "6f01a04e-cbdc-4211-9538-82e1bce551a6",
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
              "id": "ad2d0d40-380a-43ee-a548-229b0e1cc2cb"
            }
          ]
        },
        {
          "id": "9901de4f-ab80-42dd-a880-18cf5195a0e6",
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
              "id": "fd97cace-0246-45e1-934c-1f976b8598bd"
            }
          ]
        },
        {
          "id": "daca3046-7a74-46c9-aa77-0660c28b782a",
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
              "id": "6816039b-04ef-42b2-a4eb-3bfe375cd8c8"
            }
          ]
        },
        {
          "id": "1ee29a00-8ebf-4ac9-947e-03bd61840e2a",
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
              "id": "86ffd9d5-73f8-403c-b928-41dbb3f5fc9e"
            }
          ]
        }
      ]
    }
  ]
}