{
  "info": {
    "name": "AWS Internet of Things API Delete Registration Code",
    "_postman_id": "2c0a4523-94dc-4abe-8030-18312fe6ce88",
    "description": "Deletes a CA certificate registration code.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Certificate Transfers",
      "item": [
        {
          "id": "49ae5951-a0c7-4dcc-b34d-558b657ebe15",
          "name": "acceptCertificateTransfer",
          "request": {
            "url": "http://example.com/api/?Action=AcceptCertificateTransfer?certificateId=certificateId&setAsActive=setAsActive",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Accepts a pending certificate transfer."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "086099ec-c93b-4863-b6b0-5fefddcbaace"
            }
          ]
        },
        {
          "id": "f5e5f7af-f57e-4c37-b0be-9bdd88e2df7c",
          "name": "cancelCertificateTransfer",
          "request": {
            "url": "http://example.com/api/?Action=CancelCertificateTransfer?certificateId=certificateId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a pending transfer for the specified certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "08710005-c580-4df6-a683-9a9b65d89801"
            }
          ]
        }
      ]
    },
    {
      "name": "Principal Policies",
      "item": [
        {
          "id": "54763f19-ab18-4561-8f76-6b0d03342d55",
          "name": "attachPrincipalPolicy",
          "request": {
            "url": "http://example.com/api/?Action=AttachPrincipalPolicy?policyName=policyName&principal=principal",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified policy to the specified principal (certificate or other credential)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e18fb73-271f-4fbb-a6ca-489bf2b9187d"
            }
          ]
        }
      ]
    },
    {
      "name": "Thing Principals",
      "item": [
        {
          "id": "09370431-f0f9-4add-87c0-9446af0d966d",
          "name": "attachThingPrincipal",
          "request": {
            "url": "http://example.com/api/?Action=AttachThingPrincipal?principal=principal&thingName=thingName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Attaches the specified principal to the specified thing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61a61db1-16c6-4f2d-b0e3-0460ac97229c"
            }
          ]
        }
      ]
    },
    {
      "name": "Certificates",
      "item": [
        {
          "id": "eb584289-165d-414e-8f20-ab0c348eddae",
          "name": "createCertificateFromCsr",
          "request": {
            "url": "http://example.com/api/?Action=CreateCertificateFromCsr?certificateSigningRequest=certificateSigningRequest&setAsActive=setAsActive",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an X."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4529e570-fd7e-4060-8a73-fc9f0c3407fa"
            }
          ]
        },
        {
          "id": "83ed511f-fe66-47ee-a36d-b7e1ba4cb015",
          "name": "deleteCertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCertificate?certificateId=certificateId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c5b198e-8921-4442-99cf-7a55e7986a5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Keys And Certificates",
      "item": [
        {
          "id": "f24f2d01-c12f-475a-b519-fffe897d041d",
          "name": "createKeysAndCertificate",
          "request": {
            "url": "http://example.com/api/?Action=CreateKeysAndCertificate?setAsActive=setAsActive",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a 2048-bit RSA key pair and issues an X."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd629618-cab4-400f-bc5d-5366c8be1cc4"
            }
          ]
        }
      ]
    },
    {
      "name": "Policies",
      "item": [
        {
          "id": "0639b021-b904-4718-af2e-a15950267dde",
          "name": "createPolicy",
          "request": {
            "url": "http://example.com/api/?Action=CreatePolicy?policyDocument=policyDocument&policyName=policyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AWS IoT policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd3ebb12-be06-413c-aa6a-d50b4cd90408"
            }
          ]
        },
        {
          "id": "682ea034-dfb3-4e9f-9899-a059d02eee8a",
          "name": "createPolicyVersion",
          "request": {
            "url": "http://example.com/api/?Action=CreatePolicyVersion?policyDocument=policyDocument&policyName=policyName&setAsDefault=setAsDefault",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new version of the specified AWS IoT policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fd4f549b-3541-489a-b05d-64be7539fc84"
            }
          ]
        },
        {
          "id": "4c07125e-e7a2-44d3-80bb-33845026960a",
          "name": "deletePolicy",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicy?policyName=policyName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1311eb67-5e88-4066-be2d-c168a0d99989"
            }
          ]
        },
        {
          "id": "f1b4edbd-c3f3-42b6-b980-d8662404d780",
          "name": "deletePolicyVersion",
          "request": {
            "url": "http://example.com/api/?Action=DeletePolicyVersion?policyName=policyName&policyVersionId=policyVersionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified version of the specified policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7a6e5e4-45b5-4b99-8782-d02500dae793"
            }
          ]
        }
      ]
    },
    {
      "name": "Things",
      "item": [
        {
          "id": "cd18f4c2-b2cd-4483-9b84-866a24c82472",
          "name": "createThing",
          "request": {
            "url": "http://example.com/api/?Action=CreateThing?attributePayload=attributePayload&thingName=thingName&thingTypeName=thingTypeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a thing record in the thing registry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "95bf1fdf-63db-4426-bc28-340733601939"
            }
          ]
        }
      ]
    },
    {
      "name": "Thing Types",
      "item": [
        {
          "id": "45bb14d1-2715-4637-806a-3071e0619180",
          "name": "createThingType",
          "request": {
            "url": "http://example.com/api/?Action=CreateThingType?thingTypeName=thingTypeName&thingTypeProperties=thingTypeProperties",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new thing type."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5e1abe66-8a23-456d-b33d-27814b3c466f"
            }
          ]
        }
      ]
    },
    {
      "name": "Topic Rules",
      "item": [
        {
          "id": "9828dc6a-c35e-42ea-be82-99ba8c495ea2",
          "name": "createTopicRule",
          "request": {
            "url": "http://example.com/api/?Action=CreateTopicRule?ruleName=ruleName&topicRulePayload=topicRulePayload",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b8e9b43-8dd9-48e5-a317-c260995ddebf"
            }
          ]
        }
      ]
    },
    {
      "name": "CA Certificates",
      "item": [
        {
          "id": "cc5df8dc-c609-4a3c-9541-cb9cc0f4c551",
          "name": "deleteCACertificate",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCACertificate?certificateId=certificateId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a registered CA certificate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a43906a1-e9fb-42b9-a4d1-d3c921631a91"
            }
          ]
        }
      ]
    },
    {
      "name": "Registration Codes",
      "item": [
        {
          "id": "79d049e9-5f1c-4838-bb7e-4954f4b4ce8c",
          "name": "deleteRegistrationCode",
          "request": {
            "url": "http://example.com/api/?Action=DeleteRegistrationCode",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a CA certificate registration code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22a1ade9-9233-4535-aa8b-ba631b7ad9ec"
            }
          ]
        }
      ]
    }
  ]
}