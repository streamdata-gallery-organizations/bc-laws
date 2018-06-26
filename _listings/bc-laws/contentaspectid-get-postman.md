{
  "info": {
    "name": "BC Laws Describes the documents and directories available within a specific 'aspect' (content group) of the BCLaws library",
    "_postman_id": "946d2e84-499e-427f-a339-6c6e15340728",
    "description": "Describes the documents and directories available within a specific 'aspect' (content group) of the BCLaws library",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Content",
      "item": [
        {
          "id": "e42e4dd1-48b8-44da-ad63-7f971a11d4d6",
          "name": "getContentAspect",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "content/:aspectId"
              ],
              "variable": [
                {
                  "id": "aspectId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the documents and directories available within a specific 'aspect' (content group) of the BCLaws library"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ecc6f787-016b-4ffc-8d63-6a6e6218dd40"
            }
          ]
        }
      ]
    }
  ]
}