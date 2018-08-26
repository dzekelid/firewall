---
swagger: "2.0"
x-collection-name: Azure SQL Database
x-complete: 1
info:
  title: Azure SQL Database
  description: provides-create-read-update-and-delete-functionality-for-azure-sql-database-resources-including-servers-databases-elastic-pools-recommendations-operations-and-usage-metrics-
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/firewallRules/{firewallRuleName}
  : put:
      summary: Firewall Rules Create Or Update
      description: Creates or updates a firewall rule.
      operationId: FirewallRules_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-put
      parameters:
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for creating or updating a firewall rule
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Firewall Rules
    delete:
      summary: Firewall Rules Delete
      description: Deletes a firewall rule.
      operationId: FirewallRules_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-delete
      parameters:
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Firewall Rules
    get:
      summary: Firewall Rules Get
      description: Gets a firewall rule.
      operationId: FirewallRules_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-get
      parameters:
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Firewall Rules
---