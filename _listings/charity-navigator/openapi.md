swagger: "2.0"
x-collection-name: Charity Navigator
x-complete: 1
info:
  title: CharityNavigatorDataAPI
  description: the-charity-navigator-data-api-provides-access-to-charity-navigatorsratings-research-content-and-charitable-organization-profiles-
  version: 1.0.0
host: api.data.charitynavigator.org
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Categories:
    get:
      summary: Get Categories
      description: |-
        Returns metadata for Charity Navigator's classification hierarchy for
        charitable Organizations. Category is the top-level classifier, and each
        category may contain a number of Causes. <br/> ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getCategories
      x-api-path-slug: categories-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      responses:
        200:
          description: OK
      tags:
      - Categories