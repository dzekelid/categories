{
  "info": {
    "name": "Spotify Browse Categories",
    "_postman_id": "ade5a79d-f3f2-45d0-92d2-e764703146ef",
    "description": "[Get a List of Browse Categories](https://developer.spotify.com/web-api/get-list-categories/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "d58f0e00-33ec-4a0c-a3f7-8775f3653daa",
          "name": "get-a-list-of-browse-categorieshttpsdeveloperspotifycomwebapigetlistcategories",
          "request": {
            "url": "http://api.spotify.com/v1/browse/categories?country=%7B%7D&limit=%7B%7D&locale=%7B%7D&offset=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "It is used to set specified media type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "[Get a List of Browse Categories](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d1a95a0-c033-485f-a8c4-c0e4d758a5a2"
            }
          ]
        }
      ]
    }
  ]
}