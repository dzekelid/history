{
  "info": {
    "name": "Stripe Get Balance History",
    "_postman_id": "b222e6f7-d0ba-4d4c-b269-caf33b6d6a9d",
    "description": "Retrieves the balance transaction with the given ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "balance",
      "item": [
        {
          "id": "1342fbd8-2ee6-44b2-9474-8ab3bc79b48a",
          "name": "getBalanceHistory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.stripe.com",
              "path": [
                "v1",
                "balance/history/:id"
              ],
              "query": [
                {
                  "key": "expand",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Retrieves the balance transaction with the given ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1730416-87e7-49cf-a17f-dae4bb036c8d"
            }
          ]
        }
      ]
    }
  ]
}