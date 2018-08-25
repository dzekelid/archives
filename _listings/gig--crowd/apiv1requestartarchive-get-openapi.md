---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Request Art Archive
  version: 1.0.0
  description: Get request art archive.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/request/org/archive:
    get:
      summary: Get Request Org Archive
      description: Get request org archive.
      operationId: getApiV1RequestOrgArchive
      x-api-path-slug: apiv1requestorgarchive-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Request
      - Org
      - Archive
  /api/v1/request/art/archive:
    get:
      summary: Get Request Art Archive
      description: Get request art archive.
      operationId: getApiV1RequestArtArchive
      x-api-path-slug: apiv1requestartarchive-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Request
      - Art
      - Archive
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