---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Search Tweets
  description: returns collection of relevant Tweets matching query
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /statuses/mentions_timeline:
    get:
      summary: Mentions Timelines
      description: Returns the 20 most recent mentions for the authenticating user
      operationId: returns-the-20-most-recent-mentions-for-the-authenticating-user
      x-api-path-slug: statusesmentions-timeline-get
      parameters:
      - in: query
        name: contributor_details
        description: This parameter enhances the contributors element of the status
          response
      - in: query
        name: count
        description: Specifies the number of tweets to try and retrieve
      - in: query
        name: include_entities
        description: The entities node will be disincluded when set to false
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: since_id
        description: Returns result with an ID greater than the specified ID
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/user_timeline.json:
    get:
      summary: Show Timelines Status
      description: Returns a collection of the most recent Tweets posted by the User
      operationId: returns-a-collection-of-the-most-recent-tweets-posted-by-the-user
      x-api-path-slug: statusesuser-timelinejson-get
      parameters:
      - in: query
        name: contributor_details
        description: This paramters enhances the contributors element of the status
          response to include the screen_name of the contributor
      - in: query
        name: count
        description: Specifies the number of tweets to try and retrieve
      - in: query
        name: exclude_replies
        description: This paramters will prevent from appearing in the returned timeline
      - in: query
        name: include_rts
        description: When set to false, the timeline will strip any native retweet
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: screen_name
        description: The user screen name
        type: string
        format: string
      - in: query
        name: since_id
        description: Returns result with an ID greater than the specified ID
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/home_timeline:
    get:
      summary: Status Timeline
      description: Returns a collection of the most recent Tweets
      operationId: returns-a-collection-of-the-most-recent-tweets
      x-api-path-slug: statuseshome-timeline-get
      parameters:
      - in: query
        name: contributor_details
        description: This paramters enhances the contributors element of the status
          response to include the screen_name of the contributor
      - in: query
        name: exclude_replies
        description: This paramters will prevent from appearing in the returned timeline
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: since_id
        description: Returns result with an ID greater than the specified ID
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/retweets/{id}:
    post:
      summary: Show Retweets
      description: Retweens a tweet
      operationId: retweens-a-tweet
      x-api-path-slug: statusesretweetsid-post
      parameters:
      - in: path
        name: id
        description: The numerical ID of the desired status
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/show/{id}:
    get:
      summary: Show Retweet
      description: Retruns a single Tweet
      operationId: retruns-a-single-tweet
      x-api-path-slug: statusesshowid-get
      parameters:
      - in: path
        name: id
        description: The numerical ID of the desired status
      - in: query
        name: include_entities
        description: The entities node will be disincluded when set to false
      - in: query
        name: include_my_retweet
        description: When set to either true, t or 1, any Tweets returned that have
          been retweeted by the authenticating
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Tweets
  /statuses/destroy/{id}:
    post:
      summary: Remove Tweet
      description: Destroys the status specified by the required ID parameter
      operationId: destroys-the-status-specified-by-the-required-id-parameter
      x-api-path-slug: statusesdestroyid-post
      parameters:
      - in: path
        name: id
        description: The numerical ID of the desired status
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/update:
    post:
      summary: Update Status
      description: Updates the authenticating user's status
      operationId: updates-the-authenticating-users-status
      x-api-path-slug: statusesupdate-post
      parameters:
      - in: query
        name: display_coordinates
        description: Whether or not to put a pin on the exact coordinates a tweet
      - in: query
        name: in_reply_to_status_id
        description: The ID of an existing status
      - in: query
        name: lat
        description: The latitude of the location
      - in: query
        name: long
        description: The longitude of the location
      - in: query
        name: place_id
        description: A place in the world
      - in: query
        name: status
        description: The text of your status update
      - in: query
        name: trim_user
        description: When set to either true, t or 1, each tweet returned in a timeline
          will include a user object
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /statuses/oembed:
    get:
      summary: Oembed Statuses
      description: Returns information allowing the creation of an embedded representation
      operationId: returns-information-allowing-the-creation-of-an-embedded-representation
      x-api-path-slug: statusesoembed-get
      parameters:
      - in: query
        name: align
        description: Specifies whether the embedded Tweet should be left aligned
      - in: query
        name: hide_media
        description: Specifies whether the embedded tweet should automatically show
          the original message in the case that the embedded Tweet is a reply
      - in: query
        name: hide_thread
        description: Specifies whether the embedded Tweet html should include a script
          element pointing to widgets
      - in: query
        name: id
        description: The tweet/status id to return embed code for
      - in: query
        name: lang
        description: Languages code for the rendered embed
      - in: query
        name: maxwidth
        description: The maximum width in pixels that the embed should be rendered
          at
      - in: query
        name: related
        description: A value for the TWT related parameters
      - in: query
        name: url
        description: The encoded URL of the Tweet status to be embedded
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
  /lists/list:
    get:
      summary: List LIst
      description: Return all lists the authenticating or specified user subscribes
        to, including their own.
      operationId: return-all-lists-the-authenticating-or-specified-user-subscribes-to-including-their-own
      x-api-path-slug: listslist-get
      parameters:
      - in: query
        name: screen_name
        description: The screen name of the user for whom to return results for
      - in: query
        name: user_id
        description: The ID of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/statuses.json:
    get:
      summary: List Statuses
      description: Returns a timeline of tweets authored by memebers of the specified
        list
      operationId: returns-a-timeline-of-tweets-authored-by-memebers-of-the-specified-list
      x-api-path-slug: listsstatusesjson-get
      parameters:
      - in: query
        name: count
        description: Specifies the number of results to retrieve per page
      - in: query
        name: include_entities
        description: Entities are ON by default
      - in: query
        name: include_rts
        description: When set to either true, t or 1, the list timeline will contain
          native retweets in addition to the standard stream of tweets
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: since_id
        description: Returns results with an ID greater than the sepcified ID
      - in: query
        name: slug
        description: You can identify a list by its slug instead of its numerical
          id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/members/destroy:
    get:
      summary: Remove User From List
      description: Returns the list of memebers destroy
      operationId: returns-the-list-of-memebers-destroy
      x-api-path-slug: listsmembersdestroy-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The is of the user who wons the list being requested by a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list by its slug instrad of its numerical
          id
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/memberships:
    get:
      summary: Get Memberships
      description: Returns the lists of the specified user has been added to
      operationId: returns-the-lists-of-the-specified-user-has-been-added-to
      x-api-path-slug: listsmemberships-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: filter_to_owned_lists
        description: When set to true, t or 1, will return just lists the authenticating
          user owns
      - in: query
        name: screen_name
        description: The screen name of the user for whom to return results for
      - in: query
        name: user_id
        description: The id of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers:
    get:
      summary: List Subscribers
      description: Returns the subscribers of the specified list
      operationId: returns-the-subscribers-of-the-specified-list
      x-api-path-slug: listssubscribers-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list by its slug insted of its numerical id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/create:
    post:
      summary: Add List Subscribers
      description: Subscribes the authenticated user to the specified list
      operationId: subscribes-the-authenticated-user-to-the-specified-list
      x-api-path-slug: listssubscriberscreate-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/show:
    get:
      summary: Show List Subscribers
      description: Check if the specified user is a subscriber of the specified list
      operationId: check-if-the-specified-user-is-a-subscriber-of-the-specified-list
      x-api-path-slug: listssubscribersshow-get
      parameters:
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The is of the user who wons the list being requested by a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/destroy:
    get:
      summary: Remove List Subscribers
      description: Returns list of subscribers destroy
      operationId: returns-list-of-subscribers-destroy
      x-api-path-slug: listssubscribersdestroy-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/members/create_all:
    get:
      summary: Add Users to List
      description: Returns lists of members create_all
      operationId: returns-lists-of-members-create-all
      x-api-path-slug: listsmemberscreate-all-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/show:
    get:
      summary: Show Members
      description: Check if the specified user is a member of the specified list
      operationId: check-if-the-specified-user-is-a-member-of-the-specified-list
      x-api-path-slug: listmembersshow-get
      parameters:
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members:
    get:
      summary: Get Members
      description: Returns the members of the specified list
      operationId: returns-the-members-of-the-specified-list
      x-api-path-slug: listmembers-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/create:
    post:
      summary: Add Member
      description: Returns list of members create
      operationId: returns-list-of-members-create
      x-api-path-slug: listmemberscreate-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/destroy:
    post:
      summary: Destroy List
      description: Returns list of destroy
      operationId: returns-list-of-destroy
      x-api-path-slug: listsdestroy-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/update:
    post:
      summary: Update List
      description: Returns lists of updates
      operationId: returns-lists-of-updates
      x-api-path-slug: listsupdate-post
      parameters:
      - in: query
        name: description
        description: The description to give the list
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: mode
        description: Whether your list is public or private
      - in: query
        name: name
        description: The name for the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/create:
    post:
      summary: Create List
      description: Returns list of create
      operationId: returns-list-of-create
      x-api-path-slug: listscreate-post
      parameters:
      - in: query
        name: description
        description: The description to give the list
      - in: query
        name: mode
        description: Whether your list is public or private
      - in: query
        name: name
        description: The name for the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/show:
    get:
      summary: Show LIsts
      description: Returns list of show
      operationId: returns-list-of-show
      x-api-path-slug: listsshow-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscriptions:
    get:
      summary: Show List Subscriptions
      description: Returns list of subscriptions
      operationId: returns-list-of-subscriptions
      x-api-path-slug: listssubscriptions-get
      parameters:
      - in: query
        name: count
        description: The amount of results to return per page
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: screen_name
        description: The screen name of the user
      - in: query
        name: user_id
        description: The id of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/destroy_all:
    get:
      summary: Remove Members
      description: Returns lists of destroy all
      operationId: returns-lists-of-destroy-all
      x-api-path-slug: listmembersdestroy-all-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /direct_messages/sent:
    get:
      summary: Get Sent Direct Messages
      description: return 20 most recent direct messages sent
      operationId: return-20-most-recent-direct-messages-sent
      x-api-path-slug: direct-messagessent-get
      parameters:
      - in: query
        name: count
      - in: query
        name: include_entities
      - in: query
        name: max_id
      - in: query
        name: page
      - in: query
        name: since_id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Messages
  /direct_messages/show:
    get:
      summary: Show Direct Message
      description: returns a single direct message specified by an id
      operationId: returns-a-single-direct-message-specified-by-an-id
      x-api-path-slug: direct-messagesshow-get
      parameters:
      - in: query
        name: id
        description: ID of direct message
      responses:
        200:
          description: OK
      tags:
      - Social
      - Messages
  /search/tweets.json:
    get:
      summary: Search Tweets
      description: returns collection of relevant Tweets matching query
      operationId: returns-collection-of-relevant-tweets-matching-query
      x-api-path-slug: searchtweetsjson-get
      parameters:
      - in: query
        name: callback
        description: response will use the callback with given name
      - in: query
        name: count
        description: number of tweets to return
      - in: query
        name: geocode
        description: returns tweets by users located within given radius
      - in: query
        name: include_entities
        description: whether or not to include entities
      - in: query
        name: lang
        description: restricts tweets to a given language
      - in: query
        name: locale
        description: language of query you are sending
      - in: query
        name: max_id
        description: returns results with an ID less than/equal to specified ID
      - in: query
        name: q
        description: URL-encoded search query of 500 characters max
      - in: query
        name: result_type
        description: specifies type of search results you prefer
      - in: query
        name: since_id
        description: return results with ID greater than specified
      - in: query
        name: until
        description: returns tweets created before given date
      responses:
        200:
          description: OK
      tags:
      - Social
      - Statuses
x-streamrank:
  polling_total_time_average: "0.25"
  polling_size_download_average: "75800.73"
  streaming_total_time_average: "0.14"
  streaming_size_download_average: "39495.85"
  change_yes: "171"
  change_no: "1"
  time_percentage: "46"
  size_percentage: "48"
  change_percentage: "99"
  last_run: "2018-05-06"
  days_run: "1"
  minute_run: "0"
---