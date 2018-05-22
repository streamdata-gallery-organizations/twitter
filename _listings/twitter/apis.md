---
name: Twitter
x-slug: twitter
description: Twitter is a global real-time communications platform with 400 million
  monthly visitors to twitter.com, more than 200 million monthly active users around
  the world.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
x-kinRank: "10"
x-alexaRank: ""
tags: Twitter
created: "2018-05-22"
modified: "2018-05-22"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/apis.md
specificationVersion: "0.14"
apis:
- name: Twitter Mentions Timelines
  x-api-slug: twitter
  description: Returns the 20 most recent mentions for the authenticating user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//statuses/mentions_timeline
  tags: Social,Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesmentions-timeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesmentions-timeline-get-openapi.md
- name: Twitter Show Timelines Status
  x-api-slug: twitter
  description: Returns a collection of the most recent Tweets posted by the User
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//statuses/user_timeline.json
  tags: Social,Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesuser-timelinejson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesuser-timelinejson-get-openapi.md
- name: Twitter Status Timeline
  x-api-slug: twitter
  description: Returns a collection of the most recent Tweets
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//statuses/home_timeline
  tags: Social,Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statuseshome-timeline-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statuseshome-timeline-get-openapi.md
- name: Twitter Show Retweets
  x-api-slug: twitter
  description: Retweens a tweet
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//statuses/retweets/{id}
  tags: Social,Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesretweetsid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesretweetsid-post-openapi.md
- name: Twitter Show Retweet
  x-api-slug: twitter
  description: Retruns a single Tweet
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//statuses/show/{id}
  tags: Social,Tweets
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesshowid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesshowid-get-openapi.md
- name: Twitter Remove Tweet
  x-api-slug: twitter
  description: Destroys the status specified by the required ID parameter
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//statuses/destroy/{id}
  tags: Social,Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesdestroyid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesdestroyid-post-openapi.md
- name: Twitter Update Status
  x-api-slug: twitter
  description: Updates the authenticating user's status
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//statuses/update
  tags: Social,Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesupdate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesupdate-post-openapi.md
- name: Twitter Oembed Statuses
  x-api-slug: twitter
  description: Returns information allowing the creation of an embedded representation
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//statuses/oembed
  tags: Social,Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesoembed-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/statusesoembed-get-openapi.md
- name: Twitter List LIst
  x-api-slug: twitter
  description: Return all lists the authenticating or specified user subscribes to,
    including their own.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/list
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listslist-get-openapi.md
- name: Twitter List Statuses
  x-api-slug: twitter
  description: Returns a timeline of tweets authored by memebers of the specified
    list
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/statuses.json
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsstatusesjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsstatusesjson-get-openapi.md
- name: Twitter Remove User From List
  x-api-slug: twitter
  description: Returns the list of memebers destroy
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/members/destroy
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsmembersdestroy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsmembersdestroy-get-openapi.md
- name: Twitter Get Memberships
  x-api-slug: twitter
  description: Returns the lists of the specified user has been added to
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/memberships
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsmemberships-get-openapi.md
- name: Twitter List Subscribers
  x-api-slug: twitter
  description: Returns the subscribers of the specified list
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscribers
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscribers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscribers-get-openapi.md
- name: Twitter Add List Subscribers
  x-api-slug: twitter
  description: Subscribes the authenticated user to the specified list
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscribers/create
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscriberscreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscriberscreate-post-openapi.md
- name: Twitter Show List Subscribers
  x-api-slug: twitter
  description: Check if the specified user is a subscriber of the specified list
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscribers/show
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscribersshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscribersshow-get-openapi.md
- name: Twitter Remove List Subscribers
  x-api-slug: twitter
  description: Returns list of subscribers destroy
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscribers/destroy
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscribersdestroy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscribersdestroy-get-openapi.md
- name: Twitter Add Users to List
  x-api-slug: twitter
  description: Returns lists of members create_all
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/members/create_all
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsmemberscreate-all-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsmemberscreate-all-get-openapi.md
- name: Twitter Show Members
  x-api-slug: twitter
  description: Check if the specified user is a member of the specified list
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//list/members/show
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listmembersshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listmembersshow-get-openapi.md
- name: Twitter Get Members
  x-api-slug: twitter
  description: Returns the members of the specified list
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//list/members
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listmembers-get-openapi.md
- name: Twitter Add Member
  x-api-slug: twitter
  description: Returns list of members create
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//list/members/create
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listmemberscreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listmemberscreate-post-openapi.md
- name: Twitter Destroy List
  x-api-slug: twitter
  description: Returns list of destroy
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/destroy
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsdestroy-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsdestroy-post-openapi.md
- name: Twitter Update List
  x-api-slug: twitter
  description: Returns lists of updates
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/update
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsupdate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsupdate-post-openapi.md
- name: Twitter Create List
  x-api-slug: twitter
  description: Returns list of create
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/create
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listscreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listscreate-post-openapi.md
- name: Twitter Show LIsts
  x-api-slug: twitter
  description: Returns list of show
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/show
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listsshow-get-openapi.md
- name: Twitter Show List Subscriptions
  x-api-slug: twitter
  description: Returns list of subscriptions
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscriptions
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listssubscriptions-get-openapi.md
- name: Twitter Remove Members
  x-api-slug: twitter
  description: Returns lists of destroy all
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//list/members/destroy_all
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listmembersdestroy-all-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/listmembersdestroy-all-get-openapi.md
- name: Twitter Get Sent Direct Messages
  x-api-slug: twitter
  description: return 20 most recent direct messages sent
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//direct_messages/sent
  tags: Social,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messagessent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messagessent-get-openapi.md
- name: Twitter Show Direct Message
  x-api-slug: twitter
  description: returns a single direct message specified by an id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//direct_messages/show
  tags: Social,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messagesshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messagesshow-get-openapi.md
- name: Twitter Search Tweets
  x-api-slug: twitter
  description: returns collection of relevant Tweets matching query
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//search/tweets.json
  tags: Social,Statuses
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/searchtweetsjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/searchtweetsjson-get-openapi.md
- name: Twitter List Saved Searches
  x-api-slug: twitter
  description: Returns the authenticated user's saved search queries
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//saved_searches/list
  tags: Social,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/saved-searcheslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/saved-searcheslist-get-openapi.md
- name: Twitter Get Saved Search
  x-api-slug: twitter
  description: Retrieve the information for the saved search represented by the given
    id
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//saved_searches/show/{id}
  tags: Social,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/saved-searchesshowid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/saved-searchesshowid-get-openapi.md
- name: Twitter Create Saved Search
  x-api-slug: twitter
  description: Create a new saved search for the authenticated user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//saved_searches/create
  tags: Social,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/saved-searchescreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/saved-searchescreate-post-openapi.md
- name: Twitter Destroy Saved Search
  x-api-slug: twitter
  description: Destroy a saved search for the authenticating user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//saved_searches/destroy/{id}
  tags: Social,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/saved-searchesdestroyid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/saved-searchesdestroyid-post-openapi.md
- name: Twitter Get Direct Messages
  x-api-slug: twitter
  description: return 20 most recent direct messages sent to user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//direct_messages
  tags: Social,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messages-get-openapi.md
- name: Twitter Remove Direct Message
  x-api-slug: twitter
  description: destroys direct messages specified in required ID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//direct_messages/destroy
  tags: Social,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messagesdestroy-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messagesdestroy-post-openapi.md
- name: Twitter Create Direct Message
  x-api-slug: twitter
  description: sends a new direct message to specified user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//direct_messages/new
  tags: Social,Messages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messagesnew-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/direct-messagesnew-post-openapi.md
- name: Twitter Get Friends
  x-api-slug: twitter
  description: returns a cursored collection of user IDs followed by user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//friends/ids
  tags: Social,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendsids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendsids-get-openapi.md
- name: Twitter Get Followers
  x-api-slug: twitter
  description: returns a cursored collection of user IDs following the user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//followers/ids
  tags: Social,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/followersids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/followersids-get-openapi.md
- name: Twitter Get Friend Requests
  x-api-slug: twitter
  description: returns collection of IDs of users with pending follow request
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//friendships/incoming
  tags: Social,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsincoming-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsincoming-get-openapi.md
- name: Twitter Get Friend Requests
  x-api-slug: twitter
  description: returns collection of IDs of users with pending follow request from
    the user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//friendships/outgoing
  tags: Social,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsoutgoing-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsoutgoing-get-openapi.md
- name: Twitter Follow User
  x-api-slug: twitter
  description: allows users to follow user sepcified by ID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//friendships/create
  tags: Social,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipscreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipscreate-post-openapi.md
- name: Twitter Unfollow user
  x-api-slug: twitter
  description: allows user to unfollow user psecified by ID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//friendships/destroy
  tags: Social,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsdestroy-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsdestroy-post-openapi.md
- name: Twitter Unfollow User
  x-api-slug: twitter
  description: Allows one to enable or disable settings for specified user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//friendships/update
  tags: Social,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsupdate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsupdate-post-openapi.md
- name: Twitter Get Friends
  x-api-slug: twitter
  description: returns detailed info about relationship between two users
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//friendships/show
  tags: Social,Friends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/friendshipsshow-get-openapi.md
- name: Twitter Get Account Settings
  x-api-slug: twitter
  description: returns settings for user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//account/settings
  tags: Social,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountsettings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountsettings-get-openapi.md
- name: Twitter Update  Account Settings
  x-api-slug: twitter
  description: updates user's settings
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//account/settings
  tags: Social,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountsettings-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountsettings-post-openapi.md
- name: Twitter Update Account Deliver Service
  x-api-slug: twitter
  description: sets which device Twitter delivers updates to for user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//account/update_delivery_device
  tags: Social,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-delivery-device-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-delivery-device-post-openapi.md
- name: Twitter Update Profile
  x-api-slug: twitter
  description: sets values that users ar eable to set under Account tab
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//account/update_profile
  tags: Social,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-profile-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-profile-post-openapi.md
- name: Twitter Update Profile Background Image
  x-api-slug: twitter
  description: updates user's profile background image
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//account/update_profile_background_image
  tags: Social,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-profile-background-image-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-profile-background-image-post-openapi.md
- name: Twitter Update Profile Colors
  x-api-slug: twitter
  description: sets one or more hex values that controls color scheme
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//account/update_profile_colors
  tags: Social,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-profile-colors-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-profile-colors-post-openapi.md
- name: Twitter Update Profile Image
  x-api-slug: twitter
  description: updates user's profile image
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//account/update_profile_image
  tags: Social,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-profile-image-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/accountupdate-profile-image-post-openapi.md
- name: Twitter Block List
  x-api-slug: twitter
  description: disallows retweets and device notifications from a user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//blocks/list
  tags: Social,Block
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/blockslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/blockslist-get-openapi.md
- name: Twitter Block Users
  x-api-slug: twitter
  description: returns array of numeric user ids of blocked users
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//blocks/ids
  tags: Social,Block
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/blocksids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/blocksids-get-openapi.md
- name: Twitter Block User
  x-api-slug: twitter
  description: blocks the specified user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//blocks/create
  tags: Social,Block
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/blockscreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/blockscreate-post-openapi.md
- name: Twitter Unblock User
  x-api-slug: twitter
  description: un-blocks the specified user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//blocks/destroy
  tags: Social,Block
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/blocksdestroy-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/blocksdestroy-post-openapi.md
- name: Twitter User Lookup
  x-api-slug: twitter
  description: returns fully-hydrated user objects up to 100
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//users/lookup
  tags: Social,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/userslookup-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/userslookup-get-openapi.md
- name: Twitter Show User
  x-api-slug: twitter
  description: returns a variety of info about specified user
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//users/show
  tags: Social,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/usersshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/usersshow-get-openapi.md
- name: Twitter User Search
  x-api-slug: twitter
  description: simple relevance-based user search
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//users/search.json
  tags: Social,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/userssearchjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/userssearchjson-get-openapi.md
- name: Twitter User Contributees
  x-api-slug: twitter
  description: collection of users specified user can contribute to
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//users/contributees
  tags: Social,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/userscontributees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/userscontributees-get-openapi.md
- name: Twitter User Contributors
  x-api-slug: twitter
  description: collection of users that can contribute to specified account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//users/contributors
  tags: Social,Users
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/userscontributors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/userscontributors-get-openapi.md
- name: Twitter Get Place
  x-api-slug: twitter
  description: Returns all the information about a know place
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//geo/id/{place_id}
  tags: Places
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/geoidplace-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/geoidplace-id-get-openapi.md
- name: Twitter Get Lat / Log
  x-api-slug: twitter
  description: Given a latitude and a longitude, searches for up to 20 places that
    can be used as a place_id when updatting a status
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//geo/reverse_geoncode
  tags: Places,Search
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/georeverse-geoncode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/georeverse-geoncode-get-openapi.md
- name: Twitter Geo Search
  x-api-slug: twitter
  description: Search for places that can be attached to a statuses/updates
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//geo/search
  tags: Places,Similar
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/geosearch-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/geosearch-get-openapi.md
- name: Twitter Get Similar Places
  x-api-slug: twitter
  description: Locates places near the given coordinates which are similar in name
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//geo/similar_places
  tags: Places,Similar
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/geosimilar-places-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/geosimilar-places-get-openapi.md
- name: Twitter Get Places
  x-api-slug: twitter
  description: Create a new place object at the given latitude and logitude
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//geo/places
  tags: Places
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/geoplaces-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/geoplaces-get-openapi.md
- name: Twitter Show Place Trends
  x-api-slug: twitter
  description: Returns the top 10 trending topics for a specific WOEID
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//trends/place.json
  tags: Social,Trends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/trendsplacejson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/trendsplacejson-get-openapi.md
- name: Twitter Show Available Trends
  x-api-slug: twitter
  description: Returns the availability
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//trends/available.json
  tags: Social,Trends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/trendsavailablejson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/trendsavailablejson-get-openapi.md
- name: Twitter Show Closes Trends
  x-api-slug: twitter
  description: Returns the location that Twitter has trending topic information for
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//trends/closest.json
  tags: Social,Trends
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/trendsclosestjson-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/trendsclosestjson-get-openapi.md
- name: Twitter Report User Spam
  x-api-slug: twitter
  description: Returna users report spam
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//users/report_spam
  tags: Social,Users,Spam
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/usersreport-spam-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/usersreport-spam-post-openapi.md
- name: Twitter Help Configuration
  x-api-slug: twitter
  description: Returns the current configuration used by Twitter including twitter.com
    slugs which are not usernames
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//help/configuration
  tags: Help,Configuration
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/helpconfiguration-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/helpconfiguration-get-openapi.md
- name: Twitter Help Langues
  x-api-slug: twitter
  description: Returns the list of languages supported by Twitter along with the language
    code supported by Twitter
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//help/languages
  tags: Languages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/helplanguages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/helplanguages-get-openapi.md
- name: Twitter Help Privacy
  x-api-slug: twitter
  description: Returns Twitter's privacy policy
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//help/privacy
  tags: Terms of Service
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/helpprivacy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/helpprivacy-get-openapi.md
- name: Twitter Help Terms of Services
  x-api-slug: twitter
  description: Returns the Twitter Terms of Service
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//help/tos
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/helptos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/helptos-get-openapi.md
- name: Twitter Get Rate Limit Sttaus
  x-api-slug: twitter
  description: Returns the current rate limits for methods belonging to the specified
    resource families
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//application/rate_limit_status
  tags: Rate Limit
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/applicationrate-limit-status-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/applicationrate-limit-status-get-openapi.md
- name: Twitter
  x-api-slug: twitter
  description: Twitter is a global real-time communications platform with 400 million
    monthly visitors to twitter.com, more than 200 million monthly active users around
    the world.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/twitter-logo.png
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1
  tags: Twitter
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/twitter/master/_listings/twitter/openapi.md
x-common:
- type: x-net-library
  url: https://tweetinvi.codeplex.com/
- type: x-advertising-development-kit
  url: https://docs.fabric.io/unity/mopub/overview.html
- type: x-android-sdk
  url: https://docs.fabric.io/android/fabric/overview.html
- type: x-apple-sdk
  url: https://docs.fabric.io/apple/fabric/overview.html
- type: x-application-management
  url: https://apps.twitter.com/
- type: x-application-only-authentication
  url: https://dev.twitter.com/oauth/application-only
- type: x-authentication
  url: https://dev.twitter.com/oauth
- type: x-authentication-overview
  url: https://dev.twitter.com/oauth/overview
- type: x-base
  url: https://api.twitter.com
- type: x-best-practices
  url: https://dev.twitter.com/overview/general
- type: x-beta
  url: https://docs.fabric.io/unity/beta/overview.html
- type: x-branding
  url: https://brand.twitter.com/
- type: x-branding
  url: https://dev.twitter.com/overview/terms/display-requirements
- type: x-branding
  url: https://about.twitter.com/company/brand-assets
- type: x-case-studies
  url: https://dev.twitter.com/overview/case-studies
- type: x-change-log
  url: https://dev.twitter.com/ads/overview/recent-changes
- type: x-code-libraries
  url: https://dev.twitter.com/overview/api/twitter-libraries
- type: x-coldfusion-library
  url: http://monkehtweet.riaforge.org/
- type: x-console
  url: http://dev.twitter.com/rest/tools/console
- type: x-crunchbase
  url: http://www.crunchbase.com/company/twitter
- type: x-css-control
  url: https://dev.twitter.com/web/overview/css
- type: x-developer
  url: https://developer.twitter.com/
- type: x-blog
  url: https://dev.twitter.com/blog/
- type: x-blog-rss
  url: https://blog.twitter.com/api/blog.rss?name=developer
- type: x-documentation
  url: https://dev.twitter.com/overview/documentation
- type: x-embeddable
  url: https://dev.twitter.com/web/overview
- type: x-encryption
  url: https://dev.twitter.com/overview/api/tls
- type: x-blog
  url: https://blog.twitter.com/engineering
- type: x-blog-rss
  url: https://blog.twitter.com/api/blog.rss?name=engineering
- type: x-error-codes
  url: https://dev.twitter.com/overview/api/response-codes
- type: x-events
  url: https://dev.twitter.com/overview/events
- type: x-forum
  url: https://twittercommunity.com/
- type: x-forum
  url: https://twittercommunity.com/c/fabric
- type: x-geo-guidelines
  url: https://dev.twitter.com/overview/terms/geo-developer-guidelines
- type: x-github
  url: https://github.com/twitter
- type: x-go-library
  url: https://github.com/kurrik/twittergo
- type: x-internationalization
  url: https://dev.twitter.com/overview/general/adding-international-support-to-your-apps
- type: x-java-library
  url: https://www.github.com/twitter/hbc
- type: x-nodejs-library
  url: https://github.com/BoyCook/TwitterJSClient
- type: x-oembed
  url: https://dev.twitter.com/web/embedded-timelines/oembed
- type: x-partners
  url: https://dev.twitter.com/overview/general/official-partner-program
- type: x-php-library
  url: https://github.com/abraham/twitteroauth
- type: x-pin-based-authorization
  url: https://dev.twitter.com/oauth/pin-based
- type: x-blog
  url: https://blog.twitter.com/
- type: x-blog-rss
  url: https://blog.twitter.com/api/blog.rss?name=company
- type: x-privacy
  url: https://twitter.com/privacy?lang=en
- type: x-python-library
  url: https://github.com/bear/python-twitter
- type: x-rate-limits
  url: https://dev.twitter.com/rest/public/rate-limiting
- type: x-rate-limits-chart
  url: https://dev.twitter.com/rest/public/rate-limits
- type: x-road-map
  url: https://dev.twitter.com/ads/overview/upcoming-changes
- type: x-ruby-library
  url: https://github.com/sferik/twitter
- type: x-schema
  url: https://dev.twitter.com/overview/api/entities-in-twitter-objects
- type: x-security
  url: https://dev.twitter.com/overview/general/security-best-practices
- type: x-statistics
  url: https://docs.fabric.io/unity/answers/overview.html
- type: x-status
  url: https://dev.twitter.com/overview/status
- type: x-streaming
  url: https://dev.twitter.com/streaming/overview
- type: x-support
  url: https://support.twitter.com/
- type: x-terms-of-service
  url: https://dev.twitter.com/overview/terms
- type: x-transparency-report
  url: https://transparency.twitter.com/
- type: x-twitter
  url: https://twitter.com/twitterapi/
- type: x-twitter
  url: https://twitter.com/twittereng/
- type: x-website
  url: https://twitter.com/
- type: x-wordpress
  url: https://dev.twitter.com/web/wordpress
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---