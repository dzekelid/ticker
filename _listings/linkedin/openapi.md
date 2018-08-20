---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 1
info:
  title: LinkedIn
  description: bring-user-profiles-and-professional-networks-to-your-apps-
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
---