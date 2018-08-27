swagger: "2.0"
x-collection-name: Google Apps Admin SDK
x-complete: 1
info:
  title: Google Apps Admin SDK Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{groupId}/archive:
    post:
      summary: Archive Mail
      description: Inserts a new mail into the archive of the Google group.
      operationId: groupsmigration.archive.insert
      x-api-path-slug: groupidarchive-post
      parameters:
      - in: path
        name: groupId
        description: The group ID
      responses:
        200:
          description: OK
      tags:
      - Archives