---
swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 1
info:
  title: Compute Engine
  description: creates-and-runs-virtual-machines-on-google-cloud-platform-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/firewalls:
    get:
      summary: Get Firewalls
      description: Retrieves the list of firewall rules available to the specified
        project.
      operationId: compute.firewalls.list
      x-api-path-slug: projectglobalfirewalls-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Firewall
    post:
      summary: Create Firewall
      description: Creates a firewall rule in the specified project using the data
        included in the request.
      operationId: compute.firewalls.insert
      x-api-path-slug: projectglobalfirewalls-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Firewall
  /{project}/global/firewalls/{firewall}:
    delete:
      summary: Delete Firewall
      description: Deletes the specified firewall.
      operationId: compute.firewalls.delete
      x-api-path-slug: projectglobalfirewallsfirewall-delete
      parameters:
      - in: path
        name: firewall
        description: Name of the firewall rule to delete
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Firewall
    get:
      summary: Get Firewall
      description: Returns the specified firewall.
      operationId: compute.firewalls.get
      x-api-path-slug: projectglobalfirewallsfirewall-get
      parameters:
      - in: path
        name: firewall
        description: Name of the firewall rule to return
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Firewall
    patch:
      summary: Update Firewall
      description: Updates the specified firewall rule with the data included in the
        request. This method supports patch semantics.
      operationId: compute.firewalls.patch
      x-api-path-slug: projectglobalfirewallsfirewall-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: firewall
        description: Name of the firewall rule to update
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Firewall
    put:
      summary: Update Firewall
      description: Updates the specified firewall rule with the data included in the
        request.
      operationId: compute.firewalls.update
      x-api-path-slug: projectglobalfirewallsfirewall-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: firewall
        description: Name of the firewall rule to update
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Firewall
---