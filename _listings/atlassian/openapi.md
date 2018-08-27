swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
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
    post:
      summary: Create project category
      description: Create a project category via POST.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectCategoryResource.createProjectCategory_post
      x-api-path-slug: api2projectcategory-post
      responses:
        200:
          description: OK
      tags:
      - Project
      - Category
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
  /api/2/projectCategory/{id}:
    get:
      summary: Get project category by id
      description: Contains a representation of a project category in JSON format.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectCategoryResource.getProjectCategoryById_get
      x-api-path-slug: api2projectcategoryid-get
      parameters:
      - in: path
        name: id
        description: project category id
      responses:
        200:
          description: OK
      tags:
      - Project
      - Category
      - By
      - Id
    put:
      summary: Update project category
      description: Modify a project category via PUT. Any fields present in the PUT
        will override existing values. As a convenience, if a field is not present,
        it is silently ignored.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectCategoryResource.updateProjectCategory_put
      x-api-path-slug: api2projectcategoryid-put
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Project
      - Category
    delete:
      summary: Remove project category
      description: Delete a project category.
      operationId: com.atlassian.jira.rest.v2.issue.ProjectCategoryResource.removeProjectCategory_delete
      x-api-path-slug: api2projectcategoryid-delete
      parameters:
      - in: path
        name: id
        description: Id of the project category to delete
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Project
      - Category
  /api/2/statuscategory/{idOrKey}:
    get:
      summary: Get status category
      description: Returns a full representation of the StatusCategory having the
        given id or key
      operationId: com.atlassian.jira.rest.v2.issue.StatusCategoryResource.getStatusCategory_get
      x-api-path-slug: api2statuscategoryidorkey-get
      parameters:
      - in: path
        name: idOrKey
        description: a numeric StatusCategory id or a status category key
      responses:
        200:
          description: OK
      tags:
      - Status
      - Category