---
swagger: "2.0"
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RetrieveTapeArchive:
    get:
      summary: ' Retrieve Tape Archive '
      description: |-
        Retrieves an archived virtual tape from the virtual tape shelf (VTS) to a
                 gateway-VTL
      operationId: retrieveTapeArchive
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
      - tapes
      - archives
definitions: []
x-collection-name: AWS Storage Gateway Service
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