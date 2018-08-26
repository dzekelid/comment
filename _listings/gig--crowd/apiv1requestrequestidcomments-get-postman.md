{
  "info": {
    "name": "GIGANDCROWD Get Request Requestid Comments",
    "_postman_id": "2805f944-032b-409d-abe4-f30c2172d029",
    "description": "Get request requestid comments.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "3c7e50e4-54f4-45d4-a414-5803ded648b0",
          "name": "getApiV1RequestRequestComments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "gigandcrowd.com",
              "path": [
                "api/v1/request/:requestId/comments"
              ],
              "variable": [
                {
                  "id": "requestId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
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
            "description": "Get request requestid comments."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9c193d1-347c-43e4-960e-e059692be37b"
            }
          ]
        }
      ]
    }
  ]
}