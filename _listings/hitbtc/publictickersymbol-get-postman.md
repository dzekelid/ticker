{
  "info": {
    "name": "HitBTC Ticker For Symbol",
    "_postman_id": "85a9ae41-978a-4aba-9518-e6405aa1c94c",
    "description": "Ticker for symbol.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ticker",
      "item": [
        {
          "id": "13fcbcc0-0301-49ab-94a0-62c4eae88d76",
          "name": "getPublicTicker",
          "request": {
            "url": "{{default}}/public/ticker",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Ticker list for all symbols."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b60c3352-cd30-4dfe-9a17-1d7c006123b3"
            }
          ]
        }
      ]
    },
    {
      "name": "Tickersymbol",
      "item": [
        {
          "id": "d3e93a90-83de-4970-9cc0-0069e1b915d9",
          "name": "getPublicTickerSymbol",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "public/ticker/:symbol"
              ],
              "variable": [
                {
                  "id": "symbol",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Ticker for symbol."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1007e2fa-1cc9-4149-9f8d-16774130a0b4"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/api/2"
    }
  ]
}