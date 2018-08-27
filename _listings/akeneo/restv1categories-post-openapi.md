---
swagger: "2.0"
x-collection-name: Akeneo
x-complete: 0
info:
  title: Akeneo PIM API category
  description: Assuming that there is no "new_category" already existing
  version: 1.0.0
host: example.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/v1/asset-categories:
    get:
      summary: asset categories (2.1 only)
      description: Asset categories (2.1 only).
      operationId: RestV1AssetCategoriesGet
      x-api-path-slug: restv1assetcategories-get
      parameters:
      - in: query
        name: limit
      - in: query
        name: with_count
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Categories
      - (2
      - "1"
      - Only)
    patch:
      summary: asset categories (2.1 only)
      description: Asset categories (2.1 only).
      operationId: RestV1AssetCategoriesPatch
      x-api-path-slug: restv1assetcategories-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Categories
      - (2
      - "1"
      - Only)
    post:
      summary: asset category (2.1 only)
      description: Assuming that there is no "new_asset_category" already existing
      operationId: RestV1AssetCategoriesPost
      x-api-path-slug: restv1assetcategories-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Category
      - (2
      - "1"
      - Only)
  /rest/v1/categories:
    get:
      summary: categories
      description: Categories.
      operationId: RestV1CategoriesGet
      x-api-path-slug: restv1categories-get
      responses:
        200:
          description: OK
      tags:
      - Categories
    patch:
      summary: categories
      description: Categories.
      operationId: RestV1CategoriesPatch
      x-api-path-slug: restv1categories-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Categories
    post:
      summary: category
      description: Assuming that there is no "new_category" already existing
      operationId: RestV1CategoriesPost
      x-api-path-slug: restv1categories-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Category
  /rest/v1/asset-categories/asset_main_catalog:
    get:
      summary: asset category (2.1 only)
      description: Assuming that the given code is the code of an existing asset category
      operationId: RestV1AssetCategoriesAssetMainCatalogGet
      x-api-path-slug: restv1assetcategoriesasset-main-catalog-get
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Category
      - (2
      - "1"
      - Only)
  /rest/v1/asset-categories/new_asset_category:
    patch:
      summary: asset category (2.1 only)
      description: Asset category (2.1 only).
      operationId: RestV1AssetCategoriesNewAssetCategoryPatch
      x-api-path-slug: restv1assetcategoriesnew-asset-category-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Asset
      - Category
      - (2
      - "1"
      - Only)
  /rest/v1/categories/master:
    get:
      summary: category
      description: Assuming that the given code is the code of an existing category
      operationId: RestV1CategoriesMasterGet
      x-api-path-slug: restv1categoriesmaster-get
      responses:
        200:
          description: OK
      tags:
      - Category
  /rest/v1/categories/audio_video:
    patch:
      summary: category
      description: Category.
      operationId: RestV1CategoriesAudioVideoPatch
      x-api-path-slug: restv1categoriesaudio-video-patch
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Category
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