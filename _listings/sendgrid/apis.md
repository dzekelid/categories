---
name: SendGrid
x-slug: sendgrid
description: Delivering your transactional and marketing emails through the worlds
  largest cloud-based email delivery platform. Send with confidence.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
x-kinRank: "9"
x-alexaRank: "10000"
tags: Categories
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/sendgrid/apis.md
specificationVersion: "0.14"
apis:
- name: SendGrid - Get Categories
  x-api-slug: categories-get
  description: |-
    **This endpoint allows you to retrieve a list of all of your categories.**

    Categories can help organize your email analytics by enabling you to ???tag??? emails by type or broad topic. You can define your own custom categories. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/sendgrid/categories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/sendgrid/categories-get-openapi.md
- name: SendGrid - Get Categories Stats
  x-api-slug: categoriesstats-get
  description: |-
    **This endpoint allows you to retrieve all of your email statistics for each of your categories.**

    If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

    Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/sendgrid/categoriesstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/sendgrid/categoriesstats-get-openapi.md
- name: SendGrid - Get Categories Stats Sums
  x-api-slug: categoriesstatssums-get
  description: |-
    **This endpoint allows you to retrieve the total sum of each email statistic for every category over the given date range.**

    If you do not define any query parameters, this endpoint will return a sum for each category in groups of 10.

    Categories allow you to group your emails together according to broad topics that you define. For more information, please see our [User Guide](https://sendgrid.com/docs/User_Guide/Statistics/categories.html).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/142-sendgrid.jpg
  humanURL: http://sendgrid.com
  baseURL: https://api.sendgrid.com//v3
  tags: API LIfeyclessss, Imports, Stack Network, Stack, Technology, SaaS, Emails,
    Emails, Messages, Messages, Relative Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/sendgrid/categoriesstatssums-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/sendgrid/categoriesstatssums-get-openapi.md
x-common:
- type: x--net-library
  url: https://sendgrid.com/docs/Code_Examples/csharp.html
- type: x-api-gallery
  url: http://school.digger.api.gallery.streamdata.io
- type: x-api-stack
  url: http://sendgrid.stack.network
- type: x-base
  url: https://api.sendgrid.com
- type: x-blog
  url: http://blog.sendgrid.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/sendgrid/CDXr
- type: x-contact-form
  url: https://sendgrid.com/contact
- type: x-crunchbase
  url: http://www.crunchbase.com/company/sendgrid
- type: x-crunchbase
  url: https://crunchbase.com/organization/sendgrid
- type: x-developer
  url: https://sendgrid.com/developers
- type: x-documentation
  url: https://sendgrid.com/docs/index.html
- type: x-email
  url: privacy@sendgrid.com
- type: x-email
  url: legal@sendgrid.com
- type: x-email
  url: dpo@sendgrid.com
- type: x-forum
  url: http://support.sendgrid.com/forums
- type: x-github
  url: https://github.com/sendgrid
- type: x-go-library
  url: https://sendgrid.com/docs/Code_Examples/go.html
- type: x-ios-library
  url: https://sendgrid.com/docs/Code_Examples/ios.html
- type: x-java-library
  url: https://sendgrid.com/docs/Code_Examples/java.html
- type: x-labs
  url: http://labs.sendgrid.com/
- type: x-linkedin
  url: https://www.linkedin.com/company/sendgrid
- type: x-node-js-library
  url: https://sendgrid.com/docs/Code_Examples/nodejs.html
- type: x-partners
  url: https://sendgrid.com/partners
- type: x-perl-library
  url: https://sendgrid.com/docs/Code_Examples/perl.html
- type: x-php-library
  url: https://sendgrid.com/docs/Code_Examples/php.html
- type: x-pricing
  url: https://sendgrid.com/transactional-email/pricing
- type: x-privacy
  url: https://sendgrid.com/privacy
- type: x-python-library
  url: https://sendgrid.com/docs/Code_Examples/python.html
- type: x-ruby-library
  url: https://sendgrid.com/docs/Code_Examples/ruby.html
- type: x-security
  url: https://sendgrid.com/security
- type: x-selfservice-registration
  url: https://sendgrid.com/user/signup
- type: x-terms-of-service
  url: https://sendgrid.com/tos
- type: x-twitter
  url: https://twitter.com/SendGrid
- type: x-website
  url: http://sendgrid.com
- type: x-website
  url: https://sendgrid.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---