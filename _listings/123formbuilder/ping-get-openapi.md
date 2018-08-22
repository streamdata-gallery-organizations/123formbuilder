---
swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 0
info:
  title: 123FormBuilder Ping status
  version: 1.0.0
  description: This indicates if our servers are up and running.
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ping:
    get:
      summary: Ping status
      description: This indicates if our servers are up and running.
      operationId: this-indicates-if-our-servers-are-up-and-running
      x-api-path-slug: ping-get
      responses:
        200:
          description: OK
      tags:
      - Ping
      - Status
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