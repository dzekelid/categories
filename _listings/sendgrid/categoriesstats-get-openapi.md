---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Categories Stats
  description: |-
    **This endpoint allows you to retrieve all of your email statistics for each of your categories.**

    If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

    Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /categories:
    get:
      summary: Get Categories
      description: "**This endpoint allows you to retrieve a list of all of your categories.**\n\nCategories
        can help organize your email analytics by enabling you to \u201Ctag\u201D
        emails by type or broad topic. You can define your own custom categories.
        For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html)."
      operationId: GET_categories
      x-api-path-slug: categories-get
      parameters:
      - in: query
        name: category
        description: Allows you to perform a prefix search on this particular category
      - in: query
        name: limit
        description: The number of categories to display per page
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The point in the list that you would like to begin displaying
          results
      responses:
        200:
          description: OK
      tags:
      - Email
      - Categories
  /categories/stats:
    get:
      summary: Get Categories Stats
      description: |-
        **This endpoint allows you to retrieve all of your email statistics for each of your categories.**

        If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

        Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
      operationId: categories.stats.get
      x-api-path-slug: categoriesstats-get
      parameters:
      - in: query
        name: aggregated_by
        description: How to group the statistics
      - in: query
        name: categories
        description: The individual categories that you want to retrieve statistics
          for
      - in: query
        name: end_date
        description: The end date of the statistics to retrieve
      - in: query
        name: limit
        description: The number of results to include
      - in: query
        name: No Name
      - in: query
        name: offset
        description: The number of results to skip
      - in: query
        name: start_date
        description: The starting date of the statistics to retrieve
      responses:
        200:
          description: OK
      tags:
      - Email
      - Categories
      - Stats
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---