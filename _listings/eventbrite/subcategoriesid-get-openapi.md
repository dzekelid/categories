---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Subcategories
  description: Gets a subcategory by ID as subcategory.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /categories/{id}/:
    get:
      summary: Get Categories
      description: Gets a category by ID as category.
      operationId: getCategories
      x-api-path-slug: categoriesid-get
      responses:
        200:
          description: OK
      tags:
      - Categories
  /subcategories/:
    get:
      summary: Get Subcategories
      description: Returns a list of subcategory as subcategories.
      operationId: getSubcategories
      x-api-path-slug: subcategories-get
      responses:
        200:
          description: OK
      tags:
      - Subcategories
  /subcategories/{id}/:
    get:
      summary: Get Subcategories
      description: Gets a subcategory by ID as subcategory.
      operationId: getSubcategories
      x-api-path-slug: subcategoriesid-get
      responses:
        200:
          description: OK
      tags:
      - Subcategories
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