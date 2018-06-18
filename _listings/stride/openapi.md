---
swagger: "2.0"
x-collection-name: Stride
x-complete: 1
info:
  title: Stride
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
host: api.atlassian.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /site/{cloudId}/conversation/{conversationId}/archive:
    put:
      summary: Archive conversation
      description: Authentication required, with scope manage:conversation
      operationId: SiteConversationArchiveByCloudIdAndConversationIdPut
      x-api-path-slug: sitecloudidconversationconversationidarchive-put
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Archives
  /site/{cloudId}/conversation/{conversationId}/unarchive:
    put:
      summary: Unarchive conversation
      description: Authentication required, with scope manage:conversation
      operationId: SiteConversationUnarchiveByCloudIdAndConversationIdPut
      x-api-path-slug: sitecloudidconversationconversationidunarchive-put
      parameters:
      - in: header
        name: Accept
      - in: path
        name: cloudId
      - in: header
        name: Content-Type
      - in: path
        name: conversationId
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Site
      - Cloud
      - Conversation
      - Conversation
      - Unarchive
      - Archives
---