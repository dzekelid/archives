swagger: "2.0"
x-collection-name: CallFire
x-complete: 1
info:
  title: CallFire
  description: callfire
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /calls/broadcasts/{id}/archive:
    post:
      summary: Archive voice broadcast
      description: Archives a voice broadcast (voice broadcast will be hidden in search
        results)
      operationId: archiveVoiceBroadcast
      x-api-path-slug: callsbroadcastsidarchive-post
      parameters:
      - in: path
        name: id
        description: An id of a voice broadcast to archive
      responses:
        200:
          description: OK
      tags:
      - Calls
      - Broadcasts
      - Archive
  /texts/broadcasts/{id}/archive:
    post:
      summary: Archive text broadcast
      description: Archives a text broadcast (and hides it in the search results)
      operationId: archiveTextBroadcast
      x-api-path-slug: textsbroadcastsidarchive-post
      parameters:
      - in: path
        name: id
        description: An id of a text broadcast to archive
      responses:
        200:
          description: OK
      tags:
      - Texts
      - Broadcasts
      - Archive