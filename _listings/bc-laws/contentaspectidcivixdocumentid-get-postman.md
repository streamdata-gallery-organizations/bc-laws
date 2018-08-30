{
  "info": {
    "name": "BC Laws Lists the metadata available for the specified index or directory from the BCLaws legislative respository",
    "_postman_id": "e80f332a-0276-4828-89d7-95c456a8bc8e",
    "description": "Lists the metadata available for the specified index or directory from the BCLaws legislative respository",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Content",
      "item": [
        {
          "id": "570d3707-b9aa-49c6-b751-212ff05f6ad9",
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
              "id": "68f73859-1a13-401e-bf86-186674ddd0c8"
            }
          ]
        },
        {
          "id": "d6781298-7d5a-4c68-ba5b-5139a02f3ead",
          "name": "getContentAspectCivixdocument",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.bclaws.ca",
              "path": [
                "civix",
                "content/:aspectId/:civixDocumentId"
              ],
              "variable": [
                {
                  "id": "aspectId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "civixDocumentId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the metadata available for the specified index or directory from the BCLaws legislative respository"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "48581550-6818-4849-9511-15abc614505d"
            }
          ]
        }
      ]
    }
  ]
}