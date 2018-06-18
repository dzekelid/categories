---
swagger: "2.0"
x-collection-name: Iconfinder
x-complete: 0
info:
  title: Icon Finder List all categories
  description: List all categories sorted ascendingly by their identifier.
  termsOfService: https://developer.iconfinder.com/api/2.0/terms.html
  version: v2
host: api.iconfinder.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /categories:
    get:
      summary: List all categories
      description: List all categories sorted ascendingly by their identifier.
      operationId: getCategories
      x-api-path-slug: categories-get
      parameters:
      - in: query
        name: after
        description: identifier of the last category received
      - in: query
        name: count
      responses:
        200:
          description: OK
      tags:
      - Categories
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