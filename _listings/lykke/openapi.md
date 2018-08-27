swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/assetcategories:
    get:
      summary: Get API Asset Categories
      description: Get api asset categories.
      operationId: ApiAssetcategoriesGet
      x-api-path-slug: apiassetcategories-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Categories