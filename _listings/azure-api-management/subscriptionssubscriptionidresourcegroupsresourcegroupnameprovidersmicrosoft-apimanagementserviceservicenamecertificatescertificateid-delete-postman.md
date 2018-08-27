{
  "info": {
    "name": "Azure API Management API Certificates Delete",
    "_postman_id": "3d47d420-673c-4146-bbb2-62de74005311",
    "description": "Deletes specific certificate.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "certificates",
      "item": [
        {
          "id": "3132e6e3-2ade-4175-90fd-bc43f2a0f56e",
          "name": "Certificates_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.ApiManagement/service/:serviceName/certificates/:certificateId"
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
                  "id": "serviceName",
                  "value": "serviceName",
                  "type": "string"
                },
                {
                  "id": "certificateId",
                  "value": "certificateId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "If-Match",
                "value": "{}",
                "description": "The entity state (Etag) version of the certificate to delete",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes specific certificate"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f722ef27-c728-4803-b3f9-8bb9b5124001"
            }
          ]
        }
      ]
    }
  ]
}