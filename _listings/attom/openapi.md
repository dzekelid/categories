---
swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /business+category/lookup:
    get:
      summary: Returns business categories.
      description: This lookup is used to obtain a full list of Business Categories.
      operationId: getPOIBusinessCategoryLookup
      x-api-path-slug: businesscategorylookup-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Business
      - Categories
  /lob/lookup:
    get:
      summary: Returns lines of business categories.
      description: This lookup can be used to show the full list of Lines of Businesses
        (LOB), and which categories they belong to.
      operationId: getPOIlob
      x-api-path-slug: loblookup-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Lines
      - Of
      - Business
      - Categories
---