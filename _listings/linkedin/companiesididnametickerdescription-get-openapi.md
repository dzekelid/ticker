---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 0
info:
  title: LinkedIn Get Companies (,name,ticker,description)
  description: Get companies  (,name,ticker,description)
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/{id}:(id,name,ticker,description):
    get:
      summary: Get Companies (,name,ticker,description)
      description: Get companies  (,name,ticker,description)
      operationId: getCompanies(,name,ticker,description)
      x-api-path-slug: companiesididnametickerdescription-get
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - (
      - name
      - ticker
      - description)
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