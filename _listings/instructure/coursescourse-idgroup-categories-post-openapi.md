---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Courses API Create a Group Category
  description: Create a group category.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/group_categories:
    get:
      summary: List group categories for a context
      description: List group categories for a context.
      operationId: list-group-categories-for-a-context
      x-api-path-slug: coursescourse-idgroup-categories-get
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Group
      - Categories
    post:
      summary: Create a Group Category
      description: Create a group category.
      operationId: create-a-group-category
      x-api-path-slug: coursescourse-idgroup-categories-post
      parameters:
      - in: query
        name: auto_leader
        description: 'Assigns group leaders automatically when generating and allocating
          studentsnto groups Valid values are:nu201cfirstu201dnnthe first student
          to be allocated to a group is the leadernu201crandomu201dnna random student
          from all members is chosen as the leadernnn        n        n          Allowed
          values: first, random'
      - in: query
        name: create_group_count
        description: Create this number of groups (Course Only)
      - in: query
        name: group_limit
        description: Limit the maximum number of users in each group (Course Only)
      - in: query
        name: name
        description: Name of the group category
      - in: query
        name: self_signup
        description: Allow students to sign up for a group themselves (Course Only)
      - in: query
        name: split_group_count
        description: (Deprecated) Create this number of groups, and evenly distribute
          studentsnamong them
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Group
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