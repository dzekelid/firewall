{
  "info": {
    "name": "Azure Redis Cache API Firewall Rules List",
    "_postman_id": "3938edc6-30a8-472c-9462-2603df0a4e21",
    "description": "Gets all firewall rules in the specified redis cache.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "firewall rules",
      "item": [
        {
          "id": "2d9376a1-2030-4389-97f5-21ff46b2d9d8",
          "name": "FirewallRules_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Cache/Redis/:cacheName/firewallRules"
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
                  "id": "cacheName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets all firewall rules in the specified redis cache"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32d2b3ac-bb52-4937-a654-56ffbc677c63"
            }
          ]
        }
      ]
    }
  ]
}