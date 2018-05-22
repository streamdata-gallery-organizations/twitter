---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Show Retweet
  description: Retruns a single Tweet
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
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---