---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Places API Place Categories
  description: |-
    *Request a list of place categories available for a given location*

    A place category request can be made using the `categories/places` endpoint in the request URL and specifying the  focal point using the `at` parameter.



    * **at**  `latlng`
     \- Location of the central point for the places search.    e.g. `52.515,13.377`

    * **app_id**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

    * **app_code**  `text`
     \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

    * **Accept**  `header`

      Format to request from the server
  version: 1.0.0
host: places.demo.api.here.com
basePath: /places/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /meta/pois:
    get:
      summary: Point of Interest Categories
      description: "*Request point of interest category information*\n\nTo make a
        request for point-of-interest information, use `meta/pois` in the path of
        the request URL.\n  \n\n\n\n* **output**  `enum`\n \\- A 20 byte Base64 URL-safe
        encoded string used for the authentication of the client application.    You
        must include an `app_id` with every request.\n\n Valid values are : `json`,
        `text`\n\n* **app_id**  `text`\n \\- A 20 byte Base64 URL-safe encoded string
        used for the authentication of the client application.    You must include
        an `app_id` with every request..  \n\n* **app_code**  `text`\n \\- A 20 byte
        Base64 URL-safe encoded string used for the authentication of the client application.
        \   You must include an `app_code` with every request."
      operationId: MetaPoisGet
      x-api-path-slug: metapois-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: output
      responses:
        200:
          description: OK
      tags:
      - Point
      - Of
      - Interest
      - Categories
  /categories/places:
    get:
      summary: Place Categories
      description: |-
        *Request a list of place categories available for a given location*

        A place category request can be made using the `categories/places` endpoint in the request URL and specifying the  focal point using the `at` parameter.



        * **at**  `latlng`
         \- Location of the central point for the places search.    e.g. `52.515,13.377`

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

        * **Accept**  `header`

          Format to request from the server
      operationId: CategoriesPlacesGet
      x-api-path-slug: categoriesplaces-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: at
      responses:
        200:
          description: OK
      tags:
      - Place
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