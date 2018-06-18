---
name: Product Hunt
x-slug: product-hunt
description: Product Hunt surfaces the best new products, every day. Its a place for
  product-loving enthusiasts to share and geek out about the latest mobile apps, websites,
  hardware projects, and tech creations.
image: https://d1qb2nb5cznatu.cloudfront.net/startups/i/303943-1d6fe280010ae474ddd9f37792a6b604-medium_jpg.jpg?buster=1386178935
x-kinRank: "7"
x-alexaRank: "0"
tags: Categories
created: "2018-06-17"
modified: "2018-06-17"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/product-hunt/apis.md
specificationVersion: "0.14"
apis:
- name: Product Hunt Get Categories
  x-api-slug: product-hunt
  description: Get categories.
  image: https://d1qb2nb5cznatu.cloudfront.net/startups/i/303943-1d6fe280010ae474ddd9f37792a6b604-medium_jpg.jpg?buster=1386178935
  humanURL: http://producthunt.com
  baseURL: https://api.producthunt.com//v1//categories/{category}/posts
  tags: Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/product-hunt/categoriescategoryposts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/product-hunt/categoriescategoryposts-get-openapi.md
- name: Product Hunt
  x-api-slug: product-hunt
  description: Product Hunt surfaces the best new products, every day. Its a place
    for product-loving enthusiasts to share and geek out about the latest mobile apps,
    websites, hardware projects, and tech creations.
  image: https://d1qb2nb5cznatu.cloudfront.net/startups/i/303943-1d6fe280010ae474ddd9f37792a6b604-medium_jpg.jpg?buster=1386178935
  humanURL: http://producthunt.com
  baseURL: https://api.producthunt.com//v1
  tags: Categories
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/product-hunt/openapi.md
x-common:
- type: x-api-json--authoritative
  url: https://raw.githubusercontent.com/producthunt/producthunt-api/master/manifests/v1/apis.json
- type: x-blog
  url: https://stories.producthunt.com/
- type: x-blog-rss
  url: https://stories.producthunt.com/feed/
- type: x-github
  url: https://github.com/producthunt
- type: x-twitter
  url: https://twitter.com/producthunt
- type: x-website
  url: http://producthunt.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---