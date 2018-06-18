---
name: BC Geographical Names
x-slug: bc-geographical-names
description: Geographical names are more than labels on maps and road signs. They
  can reveal patterns of settlement, exploration and migration, and mirror outside
  influences to our history - aspects of the heritage and promise of an area that
  might otherwise be overlooked or forgotten by visitors and later generations.
image: ""
x-kinRank: "7"
x-alexaRank: "0"
tags: Categories
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/bc-geographical-names/apis.md
specificationVersion: "0.14"
apis:
- name: BC Geographical Names Get all feature categories
  x-api-slug: bc-geographical-names
  description: 'Gets a list of all feature categories used by the BC Geographical
    Names Information System (BCGNIS).  Note: there are three levels of classification
    in the BCGNIS feature taxonomy: classes, categories and types.  A type is a subset
    of a category, and a category is a subset of a class.'
  image: ""
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/bcgnws//featureCategories
  tags: FeatureCategories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/bc-geographical-names/featurecategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/bc-geographical-names/featurecategories-get-openapi.md
- name: BC Geographical Names
  x-api-slug: bc-geographical-names
  description: Geographical names are more than labels on maps and road signs. They
    can reveal patterns of settlement, exploration and migration, and mirror outside
    influences to our history - aspects of the heritage and promise of an area that
    might otherwise be overlooked or forgotten by visitors and later generations.
  image: ""
  humanURL: https://apps.gov.bc.ca/pub/bcgnws/
  baseURL: https://apps.gov.bc.ca//pub/bcgnws
  tags: Categories
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/bc-geographical-names/openapi.md
x-common:
- type: x-website
  url: https://apps.gov.bc.ca/pub/bcgnws/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---