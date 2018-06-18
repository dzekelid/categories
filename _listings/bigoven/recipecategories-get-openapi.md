---
swagger: "2.0"
x-collection-name: BigOven
x-complete: 0
info:
  title: Big Oven Get a list of recipe categories (the ID field can be used for include_cat
    in search parameters)
  description: Get a list of recipe categories (the id field can be used for include_cat
    in search parameters).
  termsOfService: Please see our [terms of service](http://api2.bigoven.com/web/documentation/termsofuse
  version: partner
host: api2.bigoven.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /recipe/categories:
    get:
      summary: Get a list of recipe categories (the ID field can be used for include_cat
        in search parameters)
      description: Get a list of recipe categories (the id field can be used for include_cat
        in search parameters).
      operationId: Recipe_Categories
      x-api-path-slug: recipecategories-get
      responses:
        200:
          description: OK
      tags:
      - Recipes
      - Recipe
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