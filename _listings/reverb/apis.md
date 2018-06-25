---
name: Reverb
x-slug: reverb
description: 'Reverb&#8217;s mission is to connect people with meaningful content.Reverb
  was created to find and connect the rich associations between words, ideas, content,
  and people. Through our products, we enhance broader knowledge around favorite topics
  by surfacing interesting information readers might not uncover on their own. We
  make tools for content understanding at every level from the single word on up.
  Wordnik: Get a full view of any word you???re interested in, with definitions, example
  sentences, related words, tweets from Twitter, pictures from Flickr, and much more.Reverb
  for Publishers: Reverb for Publishers brings relevant content to web audiences and
  surfaces additional content for publishers.Reverb for Developers: Reverb is committed
  to the open-source community and is proudly contributing infrastructure software
  to power applications and enterprises both small and gigantic. Our involvement with
  the Wordnik API, Scalatra, Swagger and Atmosphere is detailed on our site.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Categories
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/apis.md
specificationVersion: "0.14"
apis:
- name: reverb Get Categories
  x-api-slug: reverb
  description: List of supported product categories
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//categories
  tags: Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categories-get-openapi.md
- name: reverb Get Categories Flat
  x-api-slug: reverb
  description: Get categories flat.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//categories/flat
  tags: Categories,Flat
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categoriesflat-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categoriesflat-get-openapi.md
- name: reverb Get Categories Taxonomy
  x-api-slug: reverb
  description: Full taxonomy tree of categories including middle categories
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//categories/taxonomy
  tags: Categories,Taxonomy
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categoriestaxonomy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categoriestaxonomy-get-openapi.md
- name: reverb Get Categories Product Type Category
  x-api-slug: reverb
  description: Get categories product type category.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//categories/{product_type}/{category}
  tags: Categories,Product,Type,Category
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categoriesproduct-typecategory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categoriesproduct-typecategory-get-openapi.md
- name: reverb Get Categories Uu
  x-api-slug: reverb
  description: Get category details
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//categories/{uuid}
  tags: Categories,Uuid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categoriesuuid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/categoriesuuid-get-openapi.md
- name: reverb Get Csps Categories
  x-api-slug: reverb
  description: Get csps categories.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//csps/categories
  tags: Csps,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/cspscategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/cspscategories-get-openapi.md
- name: reverb Delete My Follows Categories Category Subcategory
  x-api-slug: reverb
  description: Delete my follows categories category subcategory.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/follows/categories/{category}/{subcategory}
  tags: My,Follows,Categories,Category,Subcategory
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriescategorysubcategory-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriescategorysubcategory-delete-openapi.md
- name: reverb Get My Follows Categories Category Subcategory
  x-api-slug: reverb
  description: Get my follows categories category subcategory.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/follows/categories/{category}/{subcategory}
  tags: My,Follows,Categories,Category,Subcategory
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriescategorysubcategory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriescategorysubcategory-get-openapi.md
- name: reverb Post My Follows Categories Category Subcategory
  x-api-slug: reverb
  description: Post my follows categories category subcategory.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/follows/categories/{category}/{subcategory}
  tags: My,Follows,Categories,Category,Subcategory
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriescategorysubcategory-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriescategorysubcategory-post-openapi.md
- name: reverb Delete My Follows Categories Entifier
  x-api-slug: reverb
  description: Delete my follows categories entifier.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/follows/categories/{identifier}
  tags: My,Follows,Categories,Identifier
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriesidentifier-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriesidentifier-delete-openapi.md
- name: reverb Get My Follows Categories Entifier
  x-api-slug: reverb
  description: Get my follows categories entifier.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/follows/categories/{identifier}
  tags: My,Follows,Categories,Identifier
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriesidentifier-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriesidentifier-get-openapi.md
- name: reverb Post My Follows Categories Entifier
  x-api-slug: reverb
  description: Post my follows categories entifier.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api//my/follows/categories/{identifier}
  tags: My,Follows,Categories,Identifier
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriesidentifier-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/myfollowscategoriesidentifier-post-openapi.md
- name: reverb
  x-api-slug: reverb
  description: 'Reverb&#8217;s mission is to connect people with meaningful content.Reverb
    was created to find and connect the rich associations between words, ideas, content,
    and people. Through our products, we enhance broader knowledge around favorite
    topics by surfacing interesting information readers might not uncover on their
    own. We make tools for content understanding at every level from the single word
    on up. Wordnik: Get a full view of any word you???re interested in, with definitions,
    example sentences, related words, tweets from Twitter, pictures from Flickr, and
    much more.Reverb for Publishers: Reverb for Publishers brings relevant content
    to web audiences and surfaces additional content for publishers.Reverb for Developers:
    Reverb is committed to the open-source community and is proudly contributing infrastructure
    software to power applications and enterprises both small and gigantic. Our involvement
    with the Wordnik API, Scalatra, Swagger and Atmosphere is detailed on our site.'
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/145_logo.png
  humanURL: https://helloreverb.com/app
  baseURL: https://api.reverb.com//api
  tags: Categories
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/reverb/openapi.md
x-common:
- type: x-blog
  url: http://blog.helloreverb.com/
- type: x-blog-rss
  url: http://blog.helloreverb.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/reverb-technologies
- type: x-github
  url: https://github.com/reverb
- type: x-twitter
  url: https://twitter.com/reverb
- type: x-website
  url: https://helloreverb.com/app
- type: x-website
  url: http://reverb.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---