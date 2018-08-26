{
  "info": {
    "name": "My News Desk Pressroom List Create Comment",
    "_postman_id": "5592028b-9baf-4e00-bd3d-10e6542d147c",
    "description": "Create Comment",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Comment",
      "item": [
        {
          "id": "7f2f17c0-8cf8-4058-9184-cd7e2df3eecc",
          "name": "getCreateComment",
          "request": {
            "url": "http://www.mynewsdesk.com/services/pressroom/create_comment/?blog=%7B%7D&body=%7B%7D&commentable_id=%7B%7D&email=%7B%7D&name=%7B%7D&type_of_media=%7B%7D&unique key=%7B%7D&user_ip=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create Comment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b269b759-5213-47ac-85a9-b159da61c8fa"
            }
          ]
        }
      ]
    }
  ]
}