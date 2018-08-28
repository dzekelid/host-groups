---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 0
info:
  title: BMC Software API Create Hostgroup
  version: 1.0.0
  description: Create a Hostgroup
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/hostgroups:
    get:
      summary: Get All Hostgroups
      description: Get all of the Hostgroups in your account
      operationId: get-all-hostgroups
      x-api-path-slug: v1hostgroups-get
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
    post:
      summary: Create Hostgroup
      description: Create a Hostgroup
      operationId: create-hostgroup
      x-api-path-slug: v1hostgroups-post
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
  /v1/hostgroups/search:
    get:
      summary: Search Hostgroups
      description: Searches the hostgroups in your account
      operationId: search-hostgroups
      x-api-path-slug: v1hostgroupssearch-get
      parameters:
      - in: query
        name: |-
          name
          The hostgroup name to search for.  Currently supported search parameters:

          name - search by the name of the hostgroup
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
  /v1/hostgroups/:hostgroupId:
    get:
      summary: Get Hostgroup by Id
      description: Retrieves a single hostgroup by its id
      operationId: get-hostgroup-by-id
      x-api-path-slug: v1hostgroupshostgroupid-get
      parameters:
      - in: query
        name: |-
          hostgroupId
          The Id of the hostgroup you are requesting
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
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