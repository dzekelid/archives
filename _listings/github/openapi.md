swagger: "2.0"
x-collection-name: GitHub
x-complete: 1
info:
  title: GitHub
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/{archive_format}/{path}:
    get:
      summary: Get Repos Owner Repo Archive Format Path
      description: |-
        Get archive link.
        This method will return a 302 to a URL to download a tarball or zipball
        archive for a repository. Please make sure your HTTP framework is
        configured to follow redirects or you will need to use the Location header
        to make a second GET request.
        Note: For private repositories, these links are temporary and expire quickly.
      operationId: get-archive-linkthis-method-will-return-a-302-to-a-url-to-download-a-tarball-or-zipballarchive-for-a
      x-api-path-slug: reposownerrepoarchive-formatpath-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: archive_format
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: path
        description: Valid Git reference, defaults to master
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Archives
      - Format
      - Path