{
  "info": {
    "name": "Twitter Help Configuration",
    "_postman_id": "9b9153c1-ba79-4fc7-892b-b45df746e39f",
    "description": "Returns the current configuration used by Twitter including twitter.com slugs which are not usernames",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Social",
      "item": [
        {
          "id": "3327cf15-ad0a-411d-9aca-a12f85f7853c",
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
              "id": "425c1c89-c4d3-4a1c-98b1-d4d626ed0f24"
            }
          ]
        },
        {
          "id": "7ef702d4-4d75-43ec-ab2c-ead1f57a60e8",
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
              "id": "26db19d8-8533-4154-b0ed-aee82feb655c"
            }
          ]
        },
        {
          "id": "f55bdc3b-a82b-4730-a072-3bce36bab7b0",
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
              "id": "085a9d60-51c3-4e56-bcf7-0fa04d4c3f99"
            }
          ]
        },
        {
          "id": "48adb0b0-bdbf-456a-ae25-2169b793c9f8",
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
              "id": "848e099c-72e0-4d80-aade-bf50692c581c"
            }
          ]
        },
        {
          "id": "8968ee8a-bfaf-4590-a3fe-20156abeeaa3",
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
              "id": "2070b2e3-2a24-40cc-803a-c5efcfefc109"
            }
          ]
        },
        {
          "id": "a08688c9-bf0a-4b6e-8733-536d9562ba6c",
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
              "id": "3f0b0d43-93ae-483b-963c-1aeb4dd74122"
            }
          ]
        },
        {
          "id": "20390457-d17d-49c4-bae6-d56ecf09d3e9",
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
              "id": "704c9b68-f82f-4aa3-b233-cd15b7c7650f"
            }
          ]
        },
        {
          "id": "248052b7-38a2-4c40-98c4-955730ab1313",
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
              "id": "2cab4cfc-c0fb-473e-8a21-b11886fc2ec4"
            }
          ]
        },
        {
          "id": "e7c9ae26-faf5-4512-a7e9-79fb96e59df1",
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
              "id": "c50b5ead-7e72-4018-845a-34851a631c12"
            }
          ]
        },
        {
          "id": "ca341d13-3ea5-4ec5-a7d8-4f9dcb30c958",
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
              "id": "a480fc23-086b-4422-840a-8fe741dfac02"
            }
          ]
        },
        {
          "id": "4768f904-e6df-479f-aeaa-a2373c2b0261",
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
              "id": "83ab6a91-685f-4f41-b8eb-aa45e108a1b8"
            }
          ]
        },
        {
          "id": "8f0f6187-ee2f-4235-b781-3ff11dab7150",
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
              "id": "bd6f0ca2-5687-4a7e-9ec7-b4d3f44e597c"
            }
          ]
        },
        {
          "id": "f0250310-9569-4847-9bc8-1e58ab69e05d",
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
              "id": "34c88506-fa1a-45ca-8f13-d4333af7c850"
            }
          ]
        },
        {
          "id": "11736b54-ab1b-4d64-9289-4ce04bace52c",
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
              "id": "ae96a5f2-a37f-4bdc-b5b5-3233114fee42"
            }
          ]
        },
        {
          "id": "d6c69a59-6409-45d5-b258-1cbc936b9566",
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
              "id": "d232817c-08e2-4cda-b0c4-6e02e610eadb"
            }
          ]
        },
        {
          "id": "0120c0a1-269e-4e8a-9b39-00b9e8a1d2c8",
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
              "id": "538de3b2-42ef-4767-a3dd-e30837889ef3"
            }
          ]
        },
        {
          "id": "54d947f5-0575-425b-abcb-a3c0b5382024",
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
              "id": "8c464b52-f27f-4576-9626-e46c85483f4f"
            }
          ]
        },
        {
          "id": "8ba51ae8-19e3-4a24-b4d9-3b3ce010aae2",
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
              "id": "2514b860-cf2d-4706-b5c1-ebbeae0d8e31"
            }
          ]
        },
        {
          "id": "18b390e7-79a9-4298-ac4d-00cef7e51e81",
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
              "id": "62132ac2-2b92-4853-b320-6966ea29e9a8"
            }
          ]
        },
        {
          "id": "eac8f721-675a-4798-8e5d-8e6a3da093bd",
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
              "id": "a85f0d8f-a3a1-4287-b035-b371d52bf59a"
            }
          ]
        },
        {
          "id": "072dd7d7-24da-42b1-be6e-0b227bf9f9f2",
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
              "id": "dfb5cbbc-a162-4ec1-942d-8cb6637198c3"
            }
          ]
        },
        {
          "id": "accc7290-80fc-4f59-b019-10d102edc870",
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
              "id": "e0e18728-2785-4c53-9b31-38130a026d30"
            }
          ]
        },
        {
          "id": "3535ffb0-d90e-47d2-97b1-f06ea35d63d3",
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
              "id": "01b75308-c69d-4465-8c00-fc53e92aaf47"
            }
          ]
        },
        {
          "id": "0485f92c-bc99-4f88-904d-c77c75ddcc22",
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
              "id": "91c66598-0b08-4c85-a45d-7b3aeaca7f1f"
            }
          ]
        },
        {
          "id": "9b52b332-95d1-4efb-a298-847e8406790c",
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
              "id": "95b57942-4a25-41fd-8c00-64eebdf78f1a"
            }
          ]
        },
        {
          "id": "aac1c4c9-c241-4ad5-a223-0e785fd7c5ff",
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
              "id": "bfc9763d-952d-4c67-a068-670a4c456c8a"
            }
          ]
        },
        {
          "id": "40cf3cd5-871d-474a-bed0-e5da211f309f",
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
              "id": "665d4b60-88f7-4772-8f4e-84fc7c5a4376"
            }
          ]
        },
        {
          "id": "fbffaf69-7a55-4b03-959c-ea03f08b14bb",
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
              "id": "9c348e69-87ef-49a0-b853-431b68ae429b"
            }
          ]
        },
        {
          "id": "b4c347d2-d0b3-46e3-9dfc-eaa820786433",
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
              "id": "ab5525a9-e366-4fc5-bf6d-7ba6a4c1b3d4"
            }
          ]
        },
        {
          "id": "5e3083a6-4f7d-4716-b2b3-bc4230f63b66",
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
              "id": "14f087f7-5c2d-44df-b51c-eea1a804f5bc"
            }
          ]
        },
        {
          "id": "18d79243-c19d-456f-a182-1df4f9dbf195",
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
              "id": "fd1aad9c-320b-49ae-be84-7e481b1424c0"
            }
          ]
        },
        {
          "id": "9cd4bbda-9141-42dc-b952-cd2f196d783f",
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
              "id": "aa87b976-b847-41ce-b10f-c6d10ae5baa6"
            }
          ]
        },
        {
          "id": "824f1fbd-32c1-45b6-a3de-e8031ad4fca1",
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
              "id": "5c565e6d-e7b8-4ec2-b601-593aa9dfdd7b"
            }
          ]
        },
        {
          "id": "99cab16b-1245-4217-ab8d-beab013065af",
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
              "id": "aeac6ab0-d53f-4c3d-897e-986ca2e6640e"
            }
          ]
        },
        {
          "id": "d6a3f5eb-9614-45d6-8706-79e05a6c1107",
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
              "id": "c7a0e259-bc06-4528-b075-414f1552b374"
            }
          ]
        },
        {
          "id": "faa5cf97-f174-46a2-bd10-a3fb784c81f0",
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
              "id": "0e5140b7-885d-4948-8057-b48a4643d343"
            }
          ]
        },
        {
          "id": "9ad9ad37-d2e3-448d-b05e-bf6fef1d2c86",
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
              "id": "654f9bcf-87b9-41ad-9d25-41b6bdb1ed3b"
            }
          ]
        },
        {
          "id": "218209ff-daa9-4c95-bdff-d9c8e35cf32d",
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
              "id": "dee10b47-bff1-4777-a277-e6675513a944"
            }
          ]
        },
        {
          "id": "aee6a7a0-ee3e-49c5-81f4-9da65ac8d09e",
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
              "id": "1a402995-33ba-4fc1-8136-a614d113fbb2"
            }
          ]
        },
        {
          "id": "6f15365e-1834-4f7a-b550-7f50c8ee6ecd",
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
              "id": "5fb3abe0-e086-408d-a099-13eef45445c2"
            }
          ]
        },
        {
          "id": "261a409c-6034-46a7-a34c-efcdfb5914b9",
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
              "id": "ca80aeb9-93ab-4405-82af-014e2c7b95ef"
            }
          ]
        },
        {
          "id": "6e100dde-7681-4fb0-b302-d61906260906",
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
              "id": "0e3337f3-9e1c-462e-968a-23c08d135783"
            }
          ]
        },
        {
          "id": "6eca1706-5f4b-4d72-83c2-8e97d5edb8ac",
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
              "id": "4edaf515-fc90-4902-9e55-5e313a233720"
            }
          ]
        },
        {
          "id": "d7e8182c-ea3f-4586-a0fa-5b8e58d3f44d",
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
              "id": "460d1bbe-7741-4d7d-bc80-36cdd1f84928"
            }
          ]
        },
        {
          "id": "1a84a184-5214-43f8-9b05-acddda793d7e",
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
              "id": "2df61fac-09f0-4500-a146-dd2a48a1576c"
            }
          ]
        },
        {
          "id": "bcd35dce-5dbf-462b-a327-bcdc9e555cc4",
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
              "id": "d0b322b2-33c2-4c29-8756-ced2f3d15461"
            }
          ]
        },
        {
          "id": "884d2e09-35ee-428e-b698-d710764b561e",
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
              "id": "89ee97bb-8d75-45e7-a133-4cd39f2736e5"
            }
          ]
        },
        {
          "id": "d542a057-1143-47cf-b3dc-a92911d7916c",
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
              "id": "837967f0-a223-4622-997b-d35ad7c3e655"
            }
          ]
        },
        {
          "id": "7a4ccd3d-59b5-4e4d-8e31-e3b6a97b3d3c",
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
              "id": "a456734b-ae60-4f78-8ed6-4207b23f764b"
            }
          ]
        },
        {
          "id": "75777d25-b544-46b3-b3ef-3d3535290d26",
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
              "id": "3688cdbd-30e2-4d26-b717-16194b088e96"
            }
          ]
        },
        {
          "id": "e5c1a87b-e997-429e-a9a4-80a792e8c623",
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
              "id": "e05611d9-aa92-4ce4-99f7-7d440fee45fe"
            }
          ]
        },
        {
          "id": "19109a69-1363-4a45-a342-05592c53589f",
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
              "id": "c4367275-0f8c-4047-8c79-6800209991ac"
            }
          ]
        },
        {
          "id": "a0aeddb4-5c43-418b-9b90-a082a903f741",
          "name": "returns-array-of-numeric-user-ids-of-blocked-users",
          "request": {
            "url": "http://api.twitter.com/1.1/blocks/ids?cursor=%7B%7D&stringify_ids=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns array of numeric user ids of blocked users"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85dfa76b-2456-42a0-bed2-380ae66c7c1b"
            }
          ]
        },
        {
          "id": "ed128b04-d4d7-4576-b21b-e9a6bcc4b23d",
          "name": "blocks-the-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/blocks/create?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "blocks the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bae03450-17f6-493a-b299-29683f1c3a1c"
            }
          ]
        },
        {
          "id": "a07bb308-ee2a-4572-841b-17911a037a7f",
          "name": "unblocks-the-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/blocks/destroy?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "un-blocks the specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d857420-aaed-4a5d-a51c-fdf5d8508d3d"
            }
          ]
        },
        {
          "id": "618d59a3-9d28-4768-acc8-ac01a3c1e4c0",
          "name": "returns-fullyhydrated-user-objects-up-to-100",
          "request": {
            "url": "http://api.twitter.com/1.1/users/lookup?include_entities=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns fully-hydrated user objects up to 100"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44947c5b-8d93-49c3-8525-72bebb8b826e"
            }
          ]
        },
        {
          "id": "ccaf0a41-7988-4ecd-99d0-83353e8b3de7",
          "name": "returns-a-variety-of-info-about-specified-user",
          "request": {
            "url": "http://api.twitter.com/1.1/users/show?include_entities=%7B%7D&screen_name=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "returns a variety of info about specified user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "deb2fb6c-29b4-4d6d-9286-e870e74d62ba"
            }
          ]
        },
        {
          "id": "8044d715-fbaa-4a50-a7c5-91d405a6e5ea",
          "name": "simple-relevancebased-user-search",
          "request": {
            "url": "http://api.twitter.com/1.1/users/search.json?count=%7B%7D&include_entities=%7B%7D&page=%7B%7D&q=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "simple relevance-based user search"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d86de494-1ea9-4e75-96d5-639a650f6d30"
            }
          ]
        },
        {
          "id": "48b35267-0107-49ae-8d85-a94afba46d96",
          "name": "collection-of-users-specified-user-can-contribute-to",
          "request": {
            "url": "http://api.twitter.com/1.1/users/contributees?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "collection of users specified user can contribute to"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef9c4eab-7bbc-4e23-9b09-04b4414f9106"
            }
          ]
        },
        {
          "id": "32d89838-cdce-4f8b-ad52-0750a682e774",
          "name": "collection-of-users-that-can-contribute-to-specified-account",
          "request": {
            "url": "http://api.twitter.com/1.1/users/contributors?include_entities=%7B%7D&screen_name=%7B%7D&skip_status=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "collection of users that can contribute to specified account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "253a4c61-feb1-4de6-841a-9801e3e25d97"
            }
          ]
        },
        {
          "id": "86b40769-da99-48b0-9428-daf292f993d4",
          "name": "returns-the-top-10-trending-topics-for-a-specific-woeid",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/place.json?exclude=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the top 10 trending topics for a specific WOEID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c249a080-8e9a-47c3-a432-fea7ae2dac93"
            }
          ]
        },
        {
          "id": "5a724c76-f64f-4c4d-b728-b450df578568",
          "name": "returns-the-availability",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/available.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the availability"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62b45fde-a3ae-4689-8b0c-c12dbfff10d8"
            }
          ]
        },
        {
          "id": "bc029132-d5d5-4def-b783-4cb3d197fcb7",
          "name": "returns-the-location-that-twitter-has-trending-topic-information-for",
          "request": {
            "url": "http://api.twitter.com/1.1/trends/closest.json?lat=%7B%7D&long=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the location that Twitter has trending topic information for"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "14081168-257f-426e-923c-1b10a4865179"
            }
          ]
        },
        {
          "id": "e5dbf93a-3592-43d7-9f7b-045613040b40",
          "name": "returna-users-report-spam",
          "request": {
            "url": "http://api.twitter.com/1.1/users/report_spam?screen_name=%7B%7D&user_id=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Returna users report spam"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43f93b46-f09b-4a3a-aa72-1f65e97fed2f"
            }
          ]
        }
      ]
    },
    {
      "name": "Places",
      "item": [
        {
          "id": "931a6d48-3ed1-4015-b4e1-8ee5fc928a8a",
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
              "id": "308b8e22-22f4-4a73-855c-34f206ccb46c"
            }
          ]
        },
        {
          "id": "81062fb1-cc69-4ea7-94ad-a28386e8790b",
          "name": "given-a-latitude-and-a-longitude-searches-for-up-to-20-places-that-can-be-used-as-a-place-id-when-up",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/reverse_geoncode?accuracy=%7B%7D&callback=%7B%7D&granularity=%7B%7D&lat=%7B%7D&long=%7B%7D&max_results=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a latitude and a longitude, searches for up to 20 places that can be used as a place_id when updatting a status"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f25239bf-a063-4629-ae68-68417c48f812"
            }
          ]
        },
        {
          "id": "bf35212e-9c34-4b73-99bc-8deb4a726be6",
          "name": "search-for-places-that-can-be-attached-to-a-statusesupdates",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/search?accuracy=%7B%7D&attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&granularity=%7B%7D&ip=%7B%7D&lat=%7B%7D&long=%7B%7D&query=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search for places that can be attached to a statuses/updates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ade0862b-7135-4154-b852-64198ed4ad51"
            }
          ]
        },
        {
          "id": "e41891db-720c-464a-8732-f57dda2f8ddc",
          "name": "locates-places-near-the-given-coordinates-which-are-similar-in-name",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/similar_places?attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&lat=%7B%7D&long=%7B%7D&name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Locates places near the given coordinates which are similar in name"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cdbf808-3fb3-472a-aad7-76d56fb6e4b8"
            }
          ]
        },
        {
          "id": "937fc24c-6f06-4f0c-bdf7-d06b1ee91151",
          "name": "create-a-new-place-object-at-the-given-latitude-and-logitude",
          "request": {
            "url": "http://api.twitter.com/1.1/geo/places?attribute:street_address=%7B%7D&callback=%7B%7D&contained_within=%7B%7D&lat=%7B%7D&long=%7B%7D&name=%7B%7D&token=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create a new place object at the given latitude and logitude"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "756dfcb6-06b5-4fb8-aafc-c46eda909a3d"
            }
          ]
        }
      ]
    },
    {
      "name": "Help",
      "item": [
        {
          "id": "fa9d6e8b-3ff3-4102-9455-8f1b1309d1d0",
          "name": "returns-the-current-configuration-used-by-twitter-including-twittercom-slugs-which-are-not-usernames",
          "request": {
            "url": "http://api.twitter.com/1.1/help/configuration",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the current configuration used by Twitter including twitter.com slugs which are not usernames"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "556b878f-f837-4e6b-87f7-307ae9caffb2"
            }
          ]
        }
      ]
    }
  ]
}