---
swagger: "2.0"
x-collection-name: TidyHQ
x-complete: 1
info:
  title: Building Block API
  description: when-i-started-api-evangelist-i-began-tracking-on-the-elements-that-other-leading-api-providers-use-to-operate-their-api-programs-and-eventually-i-started-calling-these-building-blocks--i-keep-a-running-list-of-building-blocks-broken-down-into-groups--i-think-use-these-to-keep-track-of-which-building-blocks-companies-are-using--this-is-the-api-i-use-to-manage-these-elements-of-everyday-api-operation-
  contact:
    name: Kin Lane
    url: http://kinlane.com
    email: info@kinlane.com
  version: v1
host: buildingblock.api.kinlane.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /buildingblocks/categories/:
    get:
      summary: Get Categories for Building Block
      description: retrieve building block categories
      operationId: getBuildingBlockCategories
      x-api-path-slug: buildingblockscategories-get
      parameters:
      - in: query
        name: appid
        description: your appid for accessing the building block
      - in: query
        name: appkey
        description: your appkey for accessing the building block
      responses:
        200:
          description: OK
      tags:
      - CategoriesBuilding
      - Block
---