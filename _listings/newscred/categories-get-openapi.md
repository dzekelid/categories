---
swagger: "2.0"
x-collection-name: NewsCred
x-complete: 0
info:
  title: News Cred Categories
  description: Search for categories
  version: v1
host: api.newscred.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  categories/:
    get:
      summary: Categories
      description: Search for categories
      operationId: getCategories
      x-api-path-slug: categories-get
      parameters:
      - in: query
        name: access_key
        description: Unique API access key
      - in: query
        name: autosuggest
        description: If true, partial matches will be returned, i
      - in: query
        name: query
        description: The query string to find categories matching
      responses:
        200:
          description: OK
      tags:
      - News
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