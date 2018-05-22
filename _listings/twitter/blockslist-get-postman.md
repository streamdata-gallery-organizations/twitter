{
  "info": {
    "name": "Twitter Block List",
    "_postman_id": "07a3c406-63b3-4172-82b9-dc97fad93f1d",
    "description": "disallows retweets and device notifications from a user",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Social",
      "item": [
        {
          "id": "ecb40000-c913-4c02-82fa-9f5a6ace251b",
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
              "id": "8568c368-e9fd-49d9-a064-7bf0bed17457"
            }
          ]
        },
        {
          "id": "d88761b7-196a-4a46-8cab-a432a123700d",
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
              "id": "a9711b30-6085-4adf-9665-a69c9c187ac1"
            }
          ]
        },
        {
          "id": "c628779b-a1cd-4609-84b1-444956ac222a",
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
              "id": "34c9be4b-07fe-4311-ac8c-e489bb20ee08"
            }
          ]
        },
        {
          "id": "d0de7dc6-c40d-45ac-82ee-8111b538a6f4",
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
              "id": "dbdcca7f-e38a-463a-ab30-2c614d87295e"
            }
          ]
        },
        {
          "id": "8239efbe-0a66-4ff5-8455-bab998a8a21d",
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
              "id": "4d77554a-dc05-4b2f-b0c6-c318d487fe47"
            }
          ]
        },
        {
          "id": "817ac709-b327-4cae-8c26-4e44128dc5f2",
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
              "id": "93b6e467-2f2d-4f1a-8987-33685f1efee2"
            }
          ]
        },
        {
          "id": "278cd3ec-05f5-4794-a78b-a9fa9f338bd3",
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
              "id": "4eaf3cab-f2ba-44da-b058-27f3d5499824"
            }
          ]
        },
        {
          "id": "f284d152-3a99-4654-a701-5015674bf83b",
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
              "id": "a8b530e6-3fec-486a-92fc-4edc9ea0ea83"
            }
          ]
        },
        {
          "id": "4c63ae88-2477-4d44-8f4a-7b36a93c1ead",
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
              "id": "c678dca1-b08a-4635-8047-dfeeee2d5bbe"
            }
          ]
        },
        {
          "id": "6fe985a7-17ca-4c79-9c7e-1386560ee6da",
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
              "id": "26ba1f15-5d48-4f2c-a488-25ad97a2082f"
            }
          ]
        },
        {
          "id": "b53abf8c-92ad-4ca7-8cb9-3024f69ed620",
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
              "id": "be7daa40-aff9-483d-a54f-601d3ef795ca"
            }
          ]
        },
        {
          "id": "2b5986c6-964e-4620-b4e4-91ca72056f00",
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
              "id": "42a3226f-5c47-4279-8e10-97a6b7450359"
            }
          ]
        },
        {
          "id": "a46bf8ed-6f2d-4148-bf76-5924c3754297",
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
              "id": "a5060f3e-7450-46a0-b785-a29748ef6834"
            }
          ]
        },
        {
          "id": "1d3f8711-07e7-457c-9757-708e71f58af1",
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
              "id": "918d302e-e62e-480c-98b5-ebd9b87fdfc3"
            }
          ]
        },
        {
          "id": "8ce5c60e-7476-46f2-8926-62fc2d9ff9d7",
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
              "id": "fe20befb-a248-475d-af40-2973da04fa2c"
            }
          ]
        },
        {
          "id": "677e2220-9ca7-409a-8155-4b9bd5056d67",
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
              "id": "7144a489-4e3d-4e8d-bbdd-ea6bae278543"
            }
          ]
        },
        {
          "id": "a4812174-8964-483b-9c4f-883af8650504",
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
              "id": "5f806d43-bf0c-4ee0-a428-225a3819ae6d"
            }
          ]
        },
        {
          "id": "9f287dff-af04-4318-be07-bd1acda4b84a",
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
              "id": "cf9b5548-3c48-4528-88eb-d1baeaf68701"
            }
          ]
        },
        {
          "id": "13b0e3fc-941c-4138-97a9-6e98a613c392",
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
              "id": "c21a2667-4c24-4560-896a-3430e5842270"
            }
          ]
        },
        {
          "id": "003d16dc-bf5e-4528-8f8e-ee7ceea4c082",
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
              "id": "524a9d52-4b83-44c1-87e4-0644a13be560"
            }
          ]
        },
        {
          "id": "487d3b25-9ddd-4544-8931-59e77aca657a",
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
              "id": "ba809e94-24e8-44cd-80ed-7bcfa860d005"
            }
          ]
        },
        {
          "id": "5425be17-3a7a-40b9-bba2-40ef751f654c",
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
              "id": "50220f3e-e5a0-41be-bacc-ae6cfc47e4f7"
            }
          ]
        },
        {
          "id": "3eead80e-25c5-4a47-815a-1b059eb32026",
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
              "id": "5faa886c-99c5-46bd-b1cd-bc6e860b8988"
            }
          ]
        },
        {
          "id": "0452c9e7-e1c3-4cb9-91dc-401550d43619",
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
              "id": "59e45c43-cfcb-45dd-bb4f-e43b052370ae"
            }
          ]
        },
        {
          "id": "e5eff8d8-3f71-43e8-bafe-8162c389691a",
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
              "id": "736d6c13-7b4f-4ea1-8fb5-db708c6ce7d8"
            }
          ]
        },
        {
          "id": "a2122bb2-1aa5-43b5-b313-d061a048da41",
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
              "id": "852871e5-dbcf-4a13-a4d0-26cdc5baf875"
            }
          ]
        },
        {
          "id": "51164bd1-067e-4bc8-8500-da95231c0f74",
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
              "id": "257bcb54-c218-4048-ab59-e9fcad57ecaa"
            }
          ]
        },
        {
          "id": "4b15a6df-3d57-4697-a1fc-8079f8fa54f3",
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
              "id": "65af77d8-8d75-4948-85b2-309a5957dd60"
            }
          ]
        },
        {
          "id": "a64dd13b-5278-4890-9acf-a06f8e2e34dc",
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
              "id": "968442fa-70bd-4c99-ae5d-28db0c4bf0e4"
            }
          ]
        },
        {
          "id": "272b8fcb-f903-42e5-a18a-f191a24f4c53",
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
              "id": "128d7e65-f3cf-4c6a-978c-5563eced39bc"
            }
          ]
        },
        {
          "id": "37cd2111-4f10-4105-9ab1-ca79abcdcdd1",
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
              "id": "2e5bf4e4-d91c-4679-b93d-63cb30d20acc"
            }
          ]
        },
        {
          "id": "b3186ab2-fed9-463f-8786-91609d533a56",
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
              "id": "7c444268-d4cd-472c-823e-a6ae226f0333"
            }
          ]
        },
        {
          "id": "f3288fe4-b26f-418c-8ddf-e33168d78626",
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
              "id": "4781e989-b6b5-4750-851d-6a0419b12a02"
            }
          ]
        },
        {
          "id": "f1491571-c767-41fb-abe2-25370bf7d394",
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
              "id": "c6e76616-2ea3-4432-be13-82f7f16daadb"
            }
          ]
        },
        {
          "id": "644220c8-d8a8-4afd-8fe4-29f0a1531c24",
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
              "id": "f7eebf3f-92ae-40b0-8c26-0e656b5c4c46"
            }
          ]
        },
        {
          "id": "d5d492a7-fc6b-4510-b1f8-004006fbecd0",
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
              "id": "32d3a271-5f1f-4eb7-8635-3cf0377c7ff0"
            }
          ]
        },
        {
          "id": "d87bf6f0-fd6c-4c55-9ccb-a53b0c90525f",
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
              "id": "baa542b7-a1d6-4917-b0af-48856efddbd0"
            }
          ]
        },
        {
          "id": "6c4456b6-8125-4f6c-b365-7c2d3704225a",
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
              "id": "2f7631b8-04d5-4e38-b166-0d884859d3d3"
            }
          ]
        },
        {
          "id": "6da9f71d-c0d8-48ff-b258-07af319a0271",
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
              "id": "d2f78798-b3d2-4620-afcb-0630a833fbd6"
            }
          ]
        },
        {
          "id": "e8ec1907-6214-4263-b181-880245d9f42c",
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
              "id": "9875c943-b5cc-4a45-83a2-ca9d307f6ee3"
            }
          ]
        },
        {
          "id": "41e170a3-8835-4c17-b2ee-ed7244a0cecc",
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
              "id": "7d51274c-3db7-4944-bd7d-e768012dc0fd"
            }
          ]
        },
        {
          "id": "7dd1125a-c645-44bb-af2f-abd431a4e196",
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
              "id": "d20f8ad5-4863-459b-826b-49468705abd9"
            }
          ]
        },
        {
          "id": "d0ec658d-3544-4fd3-951f-90b2eea52dcf",
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
              "id": "1a350bdc-8f34-4bdb-9eb6-c43fdfd8c072"
            }
          ]
        },
        {
          "id": "6913aec2-d891-41f5-8932-2670e02d09c1",
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
              "id": "c7e59b76-857f-4ac8-8abe-26f5c90b3eb5"
            }
          ]
        },
        {
          "id": "6ae02d20-6882-46ce-8b98-c94451bc5ba3",
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
              "id": "bcbfd8d4-6b13-4f70-a359-df257cfb4353"
            }
          ]
        },
        {
          "id": "d1a8f849-80c4-4422-ab0e-527e6323fba4",
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
              "id": "9340f914-8ee0-4aa5-a46c-1dad4fd79b3a"
            }
          ]
        },
        {
          "id": "5b4c69d9-911b-4df5-b2e5-7add3637c229",
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
              "id": "b00d2043-81fd-43c7-b0d2-52bebeab3a18"
            }
          ]
        },
        {
          "id": "8277dfaf-25c2-4825-ac5d-1e2841111e87",
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
              "id": "fc4e3334-5091-4670-93a4-5e5c90e65510"
            }
          ]
        },
        {
          "id": "11b4a5a5-8283-4515-abee-3e1e31f3b44d",
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
              "id": "d2b18c65-08e6-49e5-bf87-da2bf176190e"
            }
          ]
        },
        {
          "id": "95ddcc56-53bb-47b0-b8e5-fd9b0c81d883",
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
              "id": "5e589c7c-76d6-46d6-a7e5-28fd1488e3de"
            }
          ]
        },
        {
          "id": "d8ed3477-6a2a-4bf4-9b3f-f505f24a0cdf",
          "name": "updates-users-profile-image",
          "request": {
            "url": "http://api.twitter.com/1.1/account/update_profile_image?skip_status=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "image",
                  "value": "{}",
                  "disabled": false,
                  "description": "image to be set as profile image"
                }
              ]
            },
            "description": "updates user's profile image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4a71e36-0949-4431-a130-81a911b796d3"
            }
          ]
        },
        {
          "id": "12233c82-f598-404a-8524-b113b38a497c",
          "name": "disallows-retweets-and-device-notifications-from-a-user",
          "request": {
            "url": "http://api.twitter.com/1.1/blocks/list?cursor=%7B%7D&include_entities=%7B%7D&skip_status=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "disallows retweets and device notifications from a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81e2eec2-16da-4653-a877-bebb01da8531"
            }
          ]
        }
      ]
    }
  ]
}