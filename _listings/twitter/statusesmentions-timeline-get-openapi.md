---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Mentions Timelines
  description: Returns the 20 most recent mentions for the authenticating user
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