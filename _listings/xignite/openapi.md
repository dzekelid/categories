---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite Statistics
  description: delivers-and-charts-more-than-1400-economical-timeseries-fom-the-federal-reserve-bank-
  version: 1.0.0
host: www.xignite.com
basePath: xStatistics.json/XigniteStatistics
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetCategoriesAndTopics:
    get:
      summary: Get Categories And Topics
      description: Get categories and topics for statistics.
      operationId: postGetcategoriesandtopics
      x-api-path-slug: getcategoriesandtopics-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Categories
      - And
      - Topics
  /GetCategories:
    get:
      summary: Get Categories
      description: Get valid categories.
      operationId: postGetcategories
      x-api-path-slug: getcategories-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Categories
---