---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Topic Categories
  description: Returns a list high level topic categories
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2/categories:
    get:
      summary: Categories
      description: Returns a list of Meetup group categories
      operationId: categories
      x-api-path-slug: 2categories-get
      parameters:
      - in: query
        name: fields
        description: Parameter for requesting optional response properties
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Categories
  /2/topic_categories:
    get:
      summary: Topic Categories
      description: Returns a list of Meetup topic categories
      operationId: topics
      x-api-path-slug: 2topic-categories-get
      parameters:
      - in: query
        name: fields
        description: Parameter for requesting optional response properties
        type: string
      - in: query
        name: lat,lon,radius
        description: Use a given lat/lon/radius (miles) to search best_topics for
          instead of using the members lat/lon
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Categories
  /find/topic_categories:
    get:
      summary: Topic Categories
      description: Returns a list high level topic categories
      operationId: topics
      x-api-path-slug: findtopic-categories-get
      parameters:
      - in: query
        name: fields
        description: A comma-limited list of optional fields to append to the response
        type: string
      - in: query
        name: lat
        description: An optional approximate latitude to center a request for best_topics
        type: string
      - in: query
        name: lon
        description: An optional approximate longitude to center a request for best_topics
        type: string
      - in: query
        name: radius
        description: An radius (in miles) to center a request for best_topics
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Search
      - Topic Categories
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