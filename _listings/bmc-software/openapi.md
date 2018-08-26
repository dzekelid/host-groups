---
swagger: "2.0"
x-collection-name: BMC Software
x-complete: 1
info:
  title: BMC Software Merged API
  version: 1.0.0
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
    put:
      summary: Update Hostgroup
      description: Update a Hostgroup
      operationId: update-hostgroup
      x-api-path-slug: v1hostgroupshostgroupid-put
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
    delete:
      summary: Delete Hostgroup
      description: Delete an hostgroup
      operationId: delete-hostgroup
      x-api-path-slug: v1hostgroupshostgroupid-delete
      parameters:
      - in: query
        name: |-
          hostgroupId
          The hostgroup to delete
          forceRemove
          Remove the hostgroup, even if it&#39;s being used by a dashboard or alarm
        type: string
      responses:
        200:
          description: OK
      tags:
      - Hostgroups
---