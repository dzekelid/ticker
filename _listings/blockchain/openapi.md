swagger: "2.0"
x-collection-name: Blockchain
x-complete: 1
info:
  title: Blockchain
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ticker:
    get:
      summary: Ticker
      description: Returns a JSON object with the currency codes as keys. "15m" is
        the 15 minutes delayed market price, "last" is the most recent market price,
        "symbol" is the currency symbol.
      operationId: getTicker
      x-api-path-slug: ticker-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Ticker