---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 0
info:
  title: Youtube Get Veocategories
  description: Returns a list of categories that can be associated with YouTube videos.
  termsOfService: https://developers.google.com/terms/
  contact:
    name: Google
    url: https://google.com
  version: 1.0.0
host: www.googleapis.com
basePath: /youtube/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /guideCategories:
    get:
      summary: Get Guecategories
      description: Returns a list of categories that can be associated with YouTube
        channels.
      operationId: getGuecategories
      x-api-path-slug: guidecategories-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter specifies the language that will be used for
          text values in the API response
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of the YouTube
          channel category ID(s) for the resource(s) that are being retrieved
      - in: query
        name: part
        description: The part parameter specifies the guideCategory resource properties
          that the API response will include
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return the list
          of guide categories available in the specified country
      responses:
        200:
          description: OK
      tags:
      - Guecategories
  /videoCategories:
    get:
      summary: Get Veocategories
      description: Returns a list of categories that can be associated with YouTube
        videos.
      operationId: getVeocategories
      x-api-path-slug: videocategories-get
      parameters:
      - in: query
        name: hl
        description: The hl parameter specifies the language that should be used for
          text values in the API response
      - in: query
        name: id
        description: The id parameter specifies a comma-separated list of video category
          IDs for the resources that you are retrieving
      - in: query
        name: part
        description: The part parameter specifies the videoCategory resource properties
          that the API response will include
      - in: query
        name: regionCode
        description: The regionCode parameter instructs the API to return the list
          of video categories available in the specified country
      responses:
        200:
          description: OK
      tags:
      - Veocategories
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