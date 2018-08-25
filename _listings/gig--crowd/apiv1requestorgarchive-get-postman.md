{
  "info": {
    "name": "GIGANDCROWD Get Request Org Archive",
    "_postman_id": "7078000b-aa9d-440a-88e9-5dde04edd778",
    "description": "Get request org archive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Request",
      "item": [
        {
          "id": "30c1ff4f-307d-4fad-b3a5-c1c544993f1b",
          "name": "getApiV1RequestOrgArchive",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/request/org/archive",
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
            "description": "Get request org archive."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0714f09c-c659-4b23-9675-6d5af31fe696"
            }
          ]
        },
        {
          "id": "9098a0fb-e8fc-4672-895b-a98277c3a842",
          "name": "getApiV1RequestArtArchive",
          "request": {
            "url": "http://gigandcrowd.com/api/v1/request/art/archive",
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
            "description": "Get request art archive."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19863411-b382-4985-a039-956a73bb307e"
            }
          ]
        }
      ]
    }
  ]
}