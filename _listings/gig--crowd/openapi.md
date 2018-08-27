swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
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