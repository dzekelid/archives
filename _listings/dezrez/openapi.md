swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accountingsystem/systembalance:
    put:
      summary: Archives the accounting system
      description: Archives the accounting system.
      operationId: AccountingSystem_ArchiveSystemByforce
      x-api-path-slug: apiaccountingsystemsystembalance-put
      parameters:
      - in: query
        name: force
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Archives
      - Accounting
      - System
  /api/group/archivegroups:
    post:
      summary: Archive groups in bulk
      description: Archive groups in bulk.
      operationId: Group_ArchiveGroupsBydeleteCommand
      x-api-path-slug: apigrouparchivegroups-post
      parameters:
      - in: body
        name: deleteCommand
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Archive
      - Groups
      - In
      - Bulk
  /api/branch/updatescheduledtaskstatus/{id}:
    post:
      summary: Update SystemStatus of ScheduledTask to Active, Inactive, Deleted or
        Archived.
      description: Update systemstatus of scheduledtask to active, inactive, deleted
        or archived..
      operationId: Branch_UpdateScheduledTaskStatusByidBysystemStatus
      x-api-path-slug: apibranchupdatescheduledtaskstatusid-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: systemStatus
      responses:
        200:
          description: OK
      tags:
      - SystemStatus
      - Of
      - ScheduledTask
      - To
      - Active
      - ""
      - Inactive
      - ""
      - D
      - Archived
  /api/negotiator/getarchived:
    get:
      summary: Get all archived Negotiators for the Agency's branch.
      description: Get all archived negotiators for the agency's branch..
      operationId: Negotiator_GetArchivedByteamIdBypageSizeBypageNumber
      x-api-path-slug: apinegotiatorgetarchived-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamId
        description: (optional) teamId to get negotiators for
      responses:
        200:
          description: OK
      tags:
      - Archived
      - Negotiatorsthe
      - Agencys
      - Branch