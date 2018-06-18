---
swagger: "2.0"
x-collection-name: YouTube
x-complete: 1
info:
  title: YouTube
  description: youtube-allows-users-to-upload-view-rate-share-add-to-favorites-report-comment-on-videos-and-subscribe-to-other-users--it-offers-a-wide-variety-of-usergenerated-and-corporate-media-videos--available-content-includes-video-clips-tv-show-clips-music-videos-short-and-documentary-films-audio-recordings-movie-trailers-live-streams-and-other-content-such-as-video-blogging-short-original-videos-and-educational-videos--most-of-the-content-on-youtube-is-uploaded-by-individuals-but-media-corporations-including-cbs-the-bbc-vevo-and-hulu-offer-some-of-their-material-via-youtube-as-part-of-the-youtube-partnership-program--unregistered-users-can-only-watch-videos-on-the-site-while-registered-users-are-permitted-to-upload-an-unlimited-number-of-videos-and-add-comments-to-videos-
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
---