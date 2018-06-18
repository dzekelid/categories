---
swagger: "2.0"
x-collection-name: NewsCred
x-complete: 1
info:
  title: News Cred
  description: returns-a-list-of-articles-according-to-the-specified-set-of-parameters-
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
---