{
  "info": {
    "name": "Capital One DevExchange Get loan by id",
    "_postman_id": "7939f8dd-3f3b-4991-af4f-da8e0ac3b76a",
    "description": "Returns the loan with the specific id",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "b0d1e8f3-e610-4b87-b8c8-c3be9adb5dff",
          "name": "returns-the-loan-with-the-specific-id",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.reimaginebanking.com",
              "path": [
                "loans/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the loan with the specific id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5af32ad9-82ff-4db6-9bb5-dbdecda4f1ac"
            }
          ]
        }
      ]
    }
  ]
}