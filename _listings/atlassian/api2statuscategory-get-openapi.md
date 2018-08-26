---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Jira Cloud API Get status categories
  description: Returns a list of all status categories
  termsOfService: http://atlassian.com/terms/
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/2/projectCategory:
    get:
      summary: Get all project categories
      description: Returns all project categories
      operationId: com.atlassian.jira.rest.v2.issue.ProjectCategoryResource.getAllProjectCategories_get
      x-api-path-slug: api2projectcategory-get
      responses:
        200:
          description: OK
      tags:
      - Project
      - Categories
  /api/2/statuscategory:
    get:
      summary: Get status categories
      description: Returns a list of all status categories
      operationId: com.atlassian.jira.rest.v2.issue.StatusCategoryResource.getStatusCategories_get
      x-api-path-slug: api2statuscategory-get
      responses:
        200:
          description: OK
      tags:
      - Status
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