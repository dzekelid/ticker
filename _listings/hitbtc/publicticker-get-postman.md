{
  "info": {
    "name": "HitBTC Ticker List For All Symbols",
    "_postman_id": "6a8a8b25-e002-4175-b762-8ecc54cacc3a",
    "description": "Ticker list for all symbols.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Ticker",
      "item": [
        {
          "id": "6a4326f9-a6df-4ee3-b6cb-9a6d3e1b65ce",
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
              "id": "fb1fea52-a448-4c0b-981e-853cbd006e84"
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