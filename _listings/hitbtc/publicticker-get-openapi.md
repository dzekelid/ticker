---
swagger: "2.0"
x-collection-name: HitBTC
x-complete: 0
info:
  title: HitBTC Ticker List For All Symbols
  description: Ticker list for all symbols.
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /public/ticker:
    get:
      summary: Ticker List For All Symbols
      description: Ticker list for all symbols.
      operationId: getPublicTicker
      x-api-path-slug: publicticker-get
      responses:
        200:
          description: OK
      tags:
      - Ticker
      - List
      - Symbols
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---