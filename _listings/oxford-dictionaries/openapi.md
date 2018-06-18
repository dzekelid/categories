---
swagger: "2.0"
x-collection-name: Oxford Dictionaries
x-complete: 1
info:
  title: Oxford Dictionaries
  description: if-youre-looking-to-enhance-your-app-or-website-with-dictionary-data-dont-compromise-on-quality--the-oxford-dictionaries-api-offers-easy-and-intuitive-access-to-oxfords-dictionary-content-which-is-trusted-around-the-world--here-at-oxford-dictionaries-home-of-the-oed-we-love-words--thats-why-we-have-experienced-lexicographers-tracking-the-living-language-delving-deep-into-our-corpora-and-monitoring-a-wide-range-of-media-in-order-to-understand-how-words-are-being-used-and-how-language-is-evolving--this-research-is-used-by-our-editors-to-write-and-edit-dictionary-entries-and-translations-meaning-were-able-to-offer-uptodate-accurate-and-reliable-lexical-content-in-multiple-languages-
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
---