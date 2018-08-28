---
swagger: "2.0"
x-collection-name: Azure Data Lake Analytics
x-complete: 0
info:
  title: Azure Data Lake Analytics API Firewall Rules Update
  description: Updates the specified firewall rule.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataLakeAnalytics/accounts/{accountName}/firewallRules/{firewallRuleName}
  : put:
      summary: Firewall Rules Create Or Update
      description: Creates or updates the specified firewall rule. During update,
        the firewall rule with the specified name will be replaced with this new firewall
        rule.
      operationId: FirewallRules_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountnamefirewallrulesfirewallrulename-put
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account to add or replace
          the firewall rule
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule to create or update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to create or update the firewall rule
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      responses:
        200:
          description: OK
      tags:
      - Firewall Rule
    patch:
      summary: Firewall Rules Update
      description: Updates the specified firewall rule.
      operationId: FirewallRules_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountnamefirewallrulesfirewallrulename-patch
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account to which to update
          the firewall rule
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule to update
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: Parameters supplied to update the firewall rule
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      responses:
        200:
          description: OK
      tags:
      - Firewall Rule
    delete:
      summary: Firewall Rules Delete
      description: Deletes the specified firewall rule from the specified Data Lake
        Analytics account
      operationId: FirewallRules_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountnamefirewallrulesfirewallrulename-delete
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account from which to delete
          the firewall rule
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule to delete
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      responses:
        200:
          description: OK
      tags:
      - Firewall Rule
    get:
      summary: Firewall Rules Get
      description: Gets the specified Data Lake Analytics firewall rule.
      operationId: FirewallRules_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountnamefirewallrulesfirewallrulename-get
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account from which to get
          the firewall rule
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule to retrieve
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      responses:
        200:
          description: OK
      tags:
      - Firewall Rule
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.DataLakeAnalytics/accounts/{accountName}/firewallRules
  : get:
      summary: Firewall Rules List By Account
      description: Lists the Data Lake Analytics firewall rules within the specified
        Data Lake Analytics account.
      operationId: FirewallRules_ListByAccount
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-datalakeanalyticsaccountsaccountnamefirewallrules-get
      parameters:
      - in: path
        name: accountName
        description: The name of the Data Lake Analytics account from which to get
          the firewall rules
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the Azure resource group that contains the Data Lake
          Analytics account
      responses:
        200:
          description: OK
      tags:
      - Firewall Rule Account
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