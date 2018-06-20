{
  "info": {
    "name": "Capital One DevExchange Delete a specific existing loan",
    "_postman_id": "6c89b0d9-ca48-4d93-aff1-9846c483b447",
    "description": "Deletes the specific loan",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "banks",
      "item": [
        {
          "id": "0e835cbd-798e-4828-8f26-e950efaa45d5",
          "name": "deletes-the-specific-loan",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specific loan"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "349cfedb-5949-4d97-863b-0b39bd355577"
            }
          ]
        }
      ]
    }
  ]
}