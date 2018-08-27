swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/categories:
    get:
      summary: Get Events Categories
      description: /events/{EVENT_ID}
      operationId: eventsevent-id
      x-api-path-slug: eventscategories-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Events
      - Categories
  /venues/categories:
    get:
      summary: Get Venues Categories
      description: /venues/add
      operationId: venuesadd
      x-api-path-slug: venuescategories-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venues
      - Categories