---
swagger: "2.0"
x-collection-name: Slack
x-complete: 0
info:
  title: Slack Archive Group
  description: Archives a private channel.
  version: 1.0.3
host: slack.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /channels.archive:
    post:
      summary: Archive Channel
      description: Archives a channel.
      operationId: channels_archive
      x-api-path-slug: channels-archive-post
      parameters:
      - in: formData
        name: channel
        description: Channel to archive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
      - Archives
  /conversations.unarchive:
    post:
      summary: Unarchve Conversation
      description: Reverses conversation archival.
      operationId: conversations_unarchive
      x-api-path-slug: conversations-unarchive-post
      parameters:
      - in: formData
        name: channel
        description: ID of conversation to unarchive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
      - Archives
  /groups.createChild:
    post:
      summary: Create Child Group
      description: Clones and archives a private channel.
      operationId: groups_createChild
      x-api-path-slug: groups-createchild-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to clone and archive
      - in: formData
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
      - archives
  /channels.unarchive:
    post:
      summary: Unarchive Channel
      description: Unarchives a channel.
      operationId: channels_unarchive
      x-api-path-slug: channels-unarchive-post
      parameters:
      - in: formData
        name: channel
        description: Channel to unarchive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Channels
      - Archives
  /groups.unarchive:
    post:
      summary: Unarchive Group
      description: Unarchives a private channel.
      operationId: groups_unarchive
      x-api-path-slug: groups-unarchive-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to unarchive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
      - Archives
  /conversations.archive:
    post:
      summary: Archive Conversation
      description: Archives a conversation.
      operationId: conversations_archive
      x-api-path-slug: conversations-archive-post
      parameters:
      - in: formData
        name: channel
        description: ID of conversation to archive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Conversations
      - Archives
  /groups.archive:
    post:
      summary: Archive Group
      description: Archives a private channel.
      operationId: groups_archive
      x-api-path-slug: groups-archive-post
      parameters:
      - in: formData
        name: channel
        description: Private channel to archive
      - in: header
        name: token
        description: Authentication token
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - Groups
      - Archives
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