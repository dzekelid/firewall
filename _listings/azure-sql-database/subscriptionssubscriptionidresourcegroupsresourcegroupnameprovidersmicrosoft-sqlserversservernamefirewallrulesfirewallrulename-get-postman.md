{
  "info": {
    "name": "Azure SQL Database API Firewall Rules Get",
    "_postman_id": "08026cdb-58b5-40bc-b068-73f6e6966893",
    "description": "Gets a firewall rule.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "firewall rules",
      "item": [
        {
          "id": "dab8403d-7fcd-45a1-929c-012fb6a23de0",
          "name": "FirewallRules_Get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a firewall rule"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5103a87b-42c5-494b-89a1-da9a2c9cc045"
            }
          ]
        }
      ]
    }
  ]
}