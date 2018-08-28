---
swagger: "2.0"
x-collection-name: Azure Redis Cache
x-complete: 0
info:
  title: Azure Redis Cache API Firewall Rules List
  description: Gets all firewall rules in the specified redis cache.
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