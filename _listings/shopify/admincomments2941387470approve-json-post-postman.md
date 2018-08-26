{
  "info": {
    "name": "Shopify Approve a comment",
    "_postman_id": "10597a21-08b7-43c4-9f68-f6593bf71a73",
    "description": "Approve a comment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "d0fd7aa6-b82a-4c2e-aa3c-b98b967ee81f",
          "name": "postAdminComments2941387470Approve.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/comments/2941387470/approve.json",
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Approve a comment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd88f3a1-55da-413c-b7cb-72cba8b26bc0"
            }
          ]
        }
      ]
    }
  ]
}