{
  "info": {
    "name": "Azure SQL Database API Firewall Rules Delete",
    "_postman_id": "a7c80e08-37cf-4e61-98df-130299ee59ac",
    "description": "Deletes a firewall rule.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "firewall rules",
      "item": [
        {
          "id": "81ac9cf2-2379-43ca-998d-405f8958206a",
          "name": "FirewallRules_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/firewallRules/:firewallRuleName"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "firewallRuleName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serverName",
                  "value": "serverName",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a firewall rule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07044d3d-ba55-41c0-a14c-6e4db7980070"
            }
          ]
        }
      ]
    }
  ]
}