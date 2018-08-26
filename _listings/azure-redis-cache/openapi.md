---
swagger: "2.0"
x-collection-name: Azure Redis Cache
x-complete: 1
info:
  title: RedisManagementClient
  description: rest-api-for-azure-redis-cache-service-
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
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Cache/Redis/{cacheName}/firewallRules:
    get:
      summary: Firewall Rules List
      description: Gets all firewall rules in the specified redis cache.
      operationId: FirewallRules_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-cacherediscachenamefirewallrules-get
      parameters:
      - in: path
        name: cacheName
        description: The name of the Redis cache
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Firewall Rules
---