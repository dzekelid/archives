---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Repository Archive
  version: 1.0.0
  description: Get an archive of the repository
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/archive:
    post:
      summary: Post Projects Archive
      description: Post projects archive.
      operationId: postV3ProjectsIdArchive
      x-api-path-slug: v3projectsidarchive-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Archive
  /v3/projects/{id}/repository/archive:
    get:
      summary: Get Projects Repository Archive
      description: Get an archive of the repository
      operationId: getV3ProjectsIdRepositoryArchive
      x-api-path-slug: v3projectsidrepositoryarchive-get
      parameters:
      - in: query
        name: format
        description: The archive format
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: sha
        description: The commit sha of the archive to be downloaded
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Repository
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