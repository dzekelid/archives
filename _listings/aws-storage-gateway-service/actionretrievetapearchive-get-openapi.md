---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Retrieve Tape Archive
  version: 1.0.0
  description: |-
    Retrieves an archived virtual tape from the virtual tape shelf (VTS) to a
             gateway-VTL.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteTapeArchive:
    get:
      summary: Delete Tape Archive
      description: Deletes the specified virtual tape from the virtual tape shelf
        (VTS).
      operationId: deleteTapeArchive
      x-api-path-slug: actiondeletetapearchive-get
      parameters:
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape to delete
          from the virtual tape         shelf (VTS)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
      - Archives
  /?Action=DescribeTapeArchives:
    get:
      summary: Describe Tape Archives
      description: |-
        Returns a description of specified virtual tapes in the virtual tape shelf
                 (VTS).
      operationId: describeTapeArchives
      x-api-path-slug: actiondescribetapearchives-get
      parameters:
      - in: query
        name: Limit
        description: Specifies that the number of virtual tapes descried be limited
          to the specified         number
        type: string
      - in: query
        name: Marker
        description: An opaque string that indicates the position at which to begin
          describing virtual         tapes
        type: string
      - in: query
        name: TapeARNs
        description: Specifies one or more unique Amazon Resource Names (ARNs) that
          represent the virtual         tapes you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tape Archives
  /?Action=RetrieveTapeArchive:
    get:
      summary: Retrieve Tape Archive
      description: |-
        Retrieves an archived virtual tape from the virtual tape shelf (VTS) to a
                 gateway-VTL.
      operationId: retrieveTapeArchive
      x-api-path-slug: actionretrievetapearchive-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway you want to retrieve
          the virtual tape         to
        type: string
      - in: query
        name: TapeARN
        description: The Amazon Resource Name (ARN) of the virtual tape you want to
          retrieve from the         virtual tape shelf (VTS)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Tapes
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