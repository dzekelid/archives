---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToAssist Remote Support Mark Recordings as Archived
  description: "This method marks a list of recordings as archived by setting their
    archived flag to \u201Ctrue.\u201D No more than 500 recordings can be marked as
    archived once.\n\nNote: Session recording must be enabled on the account in order
    to use this API method. To enable session recording, log in at https://app.gotoassist.com
    (link is external) and go to Configure > GoToAssist Settings > Enable Session
    Recording check box.\n\n  Request Parameters                    \n                      \n
    \   field        data type      description    \n    recordingIds        array
    \     A list of recordingIDs for the recordings to be archived    \n\n\nStatus
    Codes                \n                \n    Staus Code        description    \n
    \   204 No Content        Recordings have been archived    \n    400 Bad Request
    \       Request may be malformed or property may be missing or invalid    \n    403
    Forbidden        Invalid authorization header or invalid recordingIDs    \n    500
    Internal Server Error        Unexpected server error"
  version: 1.0.0
host: api.getgo.com
basePath: /G2A/rest/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /archive/recordings/archived/{recordingIDs}:
    put:
      summary: Mark Recordings as Archived
      description: "This method marks a list of recordings as archived by setting
        their archived flag to \u201Ctrue.\u201D No more than 500 recordings can be
        marked as archived once.\n\nNote: Session recording must be enabled on the
        account in order to use this API method. To enable session recording, log
        in at https://app.gotoassist.com (link is external) and go to Configure >
        GoToAssist Settings > Enable Session Recording check box.\n\n  Request Parameters
        \                   \n                      \n    field        data type      description
        \   \n    recordingIds        array      A list of recordingIDs for the recordings
        to be archived    \n\n\nStatus Codes                \n                \n    Staus
        Code        description    \n    204 No Content        Recordings have been
        archived    \n    400 Bad Request        Request may be malformed or property
        may be missing or invalid    \n    403 Forbidden        Invalid authorization
        header or invalid recordingIDs    \n    500 Internal Server Error        Unexpected
        server error"
      operationId: ArchiveRecordingsArchivedByRecordingIDsPut
      x-api-path-slug: archiverecordingsarchivedrecordingids-put
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: recordingIDs
      responses:
        200:
          description: OK
      tags:
      - Mark
      - Recordings
      - As
      - Archived
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