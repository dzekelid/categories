---
name: Spotify
x-slug: spotify
description: Spotify is a digital music service that gives you access to millions
  of songs.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
x-kinRank: "8"
x-alexaRank: "132"
tags: Categories
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/spotify/apis.md
specificationVersion: "0.14"
apis:
- name: Spotify Browse Categories
  x-api-slug: spotify
  description: '[Get a List of Browse Categories](https://developer.spotify.com/web-api/get-list-categories/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//browse/categories
  tags: Music,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/spotify/browsecategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/spotify/browsecategories-get-openapi.md
- name: Spotify Browse Category
  x-api-slug: spotify
  description: '[Get a Single Browse Category](https://developer.spotify.com/web-api/get-category/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//browse/categories/{category_id}
  tags: Music,Categories,Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/spotify/browsecategoriescategory-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/spotify/browsecategoriescategory-id-get-openapi.md
- name: Spotify
  x-api-slug: spotify
  description: Spotify is a digital music service that gives you access to millions
    of songs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1
  tags: Categories
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/categories/master/_listings/spotify/openapi.md
x-common:
- type: x-api-json--authoritative
  url: https://developer.spotify.com/wp-content/uploads/apis.json
- type: x-android-sdk
  url: https://developer.spotify.com/technologies/spotify-android-sdk/
- type: x-application-gallery
  url: https://developer.spotify.com/my-applications/
- type: x-application-gallery
  url: https://developer.spotify.com/showcase/
- type: x-base-url
  url: https://api.spotify.com
- type: x-blog
  url: http://www.spotify.com/blog/
- type: x-blog-rss
  url: http://www.spotify.com/blog/feed
- type: x-change-log
  url: https://developer.spotify.com/web-api/change-log/
- type: x-console
  url: https://developer.spotify.com/web-api/console/
- type: x-crunchbase
  url: https://crunchbase.com/organization/spotify
- type: x-crunchbase
  url: http://www.crunchbase.com/company/spotify
- type: x-developer
  url: https://developer.spotify.com/
- type: x-email
  url: office@spotify.com
- type: x-ios-sdk
  url: https://developer.spotify.com/technologies/spotify-ios-sdk/
- type: x-issues
  url: https://github.com/spotify/web-api/issues
- type: x-linkedin
  url: https://www.linkedin.com/company/spotify/
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/spotify
- type: x-terms-of-service
  url: https://developer.spotify.com/developer-terms-of-use/
- type: x-twitter
  url: https://twitter.com/SpotifyPlatform
- type: x-twitter
  url: https://twitter.com/spotify
- type: x-github
  url: https://github.com/spotify
- type: x-website
  url: http://www.spotify.com
- type: x-website
  url: http://spotify.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---