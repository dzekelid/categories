---
swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 0
info:
  title: Oxford Dictionaries Lists available lexical categories in a dataset
  description: Returns a list of available [lexical categories](documentation/glossary?term=lexicalcategory)
    for a given language dataset.
  termsOfService: http://helloreverb.com/terms/
  version: 1.8.0
host: od-api-demo.oxforddictionaries.com:443
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lexicalcategories/{language}:
    get:
      summary: Lists available lexical categories in a dataset
      description: Returns a list of available [lexical categories](documentation/glossary?term=lexicalcategory)
        for a given language dataset.
      operationId: getLexicalcategoriesLanguage
      x-api-path-slug: lexicalcategorieslanguage-get
      parameters:
      - in: path
        name: language
        description: IANA language code
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Lexicalcategories
      - Language
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