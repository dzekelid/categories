---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Breaking News API
  description: ap-breaking-news-api-allows-your-organization-to-retrieve-a-list-of-available-breaking-news-categories-and-then-request-content-for-a-specific-category-
  version: v2
host: developerapi.ap.org
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  categories.svc/:
    get:
      summary: Categories
      description: Returns a list of available AP Breaking News categories, including
        category IDs.
      operationId: getCategories.svc
      x-api-path-slug: categories-svc-get
      parameters:
      - in: query
        name: apiKey
        description: API Key
      responses:
        200:
          description: OK
      tags:
      - Categories
---