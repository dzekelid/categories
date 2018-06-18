---
swagger: "2.0"
x-collection-name: Iconfinder
x-complete: 1
info:
  title: Icon Finder
  description: give-your-users-instant-access-to-more-than-300000-icons-
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
  /v2/categories/{categoryID}:
    get:
      summary: Get category details
      description: Get details about a specific category identified by its identifier.
      operationId: getV2CategoriesCategory
      x-api-path-slug: v2categoriescategoryid-get
      parameters:
      - in: path
        name: categoryID
        description: The unique ID of the category
      responses:
        200:
          description: OK
      tags:
      - Categories
---