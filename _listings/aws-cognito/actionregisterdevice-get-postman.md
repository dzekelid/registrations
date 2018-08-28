{
  "info": {
    "name": "AWS Cognito API Register Device",
    "_postman_id": "2bcf95ad-6bde-4474-8f6d-e986b0098603",
    "description": "Registers a device to receive push sync notifications.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attributes",
      "item": [
        {
          "id": "bb2925dd-141b-4fd8-8215-1c102d50e22d",
          "name": "addCustomAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AddCustomAttributes?CustomAttributes=CustomAttributes&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds additional user attributes to the user pool schema."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e2e92d90-5a25-440f-98bc-8f41e6b3b230"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "0c485722-3457-4e54-a684-281c587290f2",
          "name": "adminAddUserToGroup",
          "request": {
            "url": "http://example.com/api/?Action=AdminAddUserToGroup?GroupName=GroupName&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds the specified user to the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4fa9ce8-afcd-4b02-94ad-b0a47485e577"
            }
          ]
        },
        {
          "id": "23675fc5-69f0-4ac9-83c7-e8dc9ea653fc",
          "name": "adminCreateUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminCreateUser?DesiredDeliveryMediums=DesiredDeliveryMediums&ForceAliasCreation=ForceAliasCreation&MessageAction=MessageAction&TemporaryPassword=TemporaryPassword&UserAttributes=UserAttributes&Username=Username&UserPoolId=UserPoolId&ValidationData=ValidationData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new user in the specified user pool and sends a welcome message via email\n            or phone (SMS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c3d9a4e-95e8-4bac-8d6b-f713cbe47d58"
            }
          ]
        },
        {
          "id": "708de81a-d78f-4ae8-88f2-4bb2ef21ceba",
          "name": "adminDeleteUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminDeleteUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d49e0fb0-0c5b-417d-bdac-68f287cf8b03"
            }
          ]
        },
        {
          "id": "c52cf81c-6297-48b5-bf7e-9de7c73bf8b5",
          "name": "adminDeleteUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AdminDeleteUserAttributes?UserAttributeNames=UserAttributeNames&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the user attributes in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e2a5874-18a8-491e-a67d-d60f601ac6e1"
            }
          ]
        },
        {
          "id": "23b52ddd-9c84-4778-9b9e-5eb021f2401a",
          "name": "adminDisableUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminDisableUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables the specified user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b5172c58-818b-4189-a545-567add99745e"
            }
          ]
        },
        {
          "id": "b02843ba-93bd-4ec8-bcbc-4306eb969c29",
          "name": "adminEnableUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminEnableUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables the specified user as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1627b3c8-9c1b-4ac4-9092-c3b1a042925d"
            }
          ]
        },
        {
          "id": "2743ba72-01b9-4048-a7ca-4bf105a60fea",
          "name": "adminGetUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminGetUser?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the specified user by user name in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5bff7ec6-b07c-4551-bc01-018a09ef067d"
            }
          ]
        },
        {
          "id": "2b197946-e50a-4d94-99f2-bb9e47e60a74",
          "name": "adminListGroupsForUser",
          "request": {
            "url": "http://example.com/api/?Action=AdminListGroupsForUser?Limit=Limit&NextToken=NextToken&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the groups that the user belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2fe7a892-7b93-4361-a4a2-52c4c59a6d3d"
            }
          ]
        },
        {
          "id": "396d2dda-f944-4239-8a03-294fbd033def",
          "name": "adminRemoveUserFromGroup",
          "request": {
            "url": "http://example.com/api/?Action=AdminRemoveUserFromGroup?GroupName=GroupName&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified user from the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "840e884b-1525-4e3e-a4c0-d5b138a6bfac"
            }
          ]
        },
        {
          "id": "eacc9328-baf4-44ff-9d63-3c099a7dee96",
          "name": "adminResetUserPassword",
          "request": {
            "url": "http://example.com/api/?Action=AdminResetUserPassword?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resets the specified user's password in a user pool as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfa6a47f-5a2e-4233-9591-063be208bde9"
            }
          ]
        },
        {
          "id": "f13cc4f0-bf31-40a1-92b0-02465a165ab2",
          "name": "adminSetUserSettings",
          "request": {
            "url": "http://example.com/api/?Action=AdminSetUserSettings?MFAOptions=MFAOptions&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets all the user settings for a specified user name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28d4aa8a-e2e5-4b28-95f5-99769b043dcc"
            }
          ]
        },
        {
          "id": "f6751c4b-806a-45a5-8dd2-169bffd7356d",
          "name": "adminUpdateDeviceStatus",
          "request": {
            "url": "http://example.com/api/?Action=AdminUpdateDeviceStatus?DeviceKey=DeviceKey&DeviceRememberedStatus=DeviceRememberedStatus&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the device status as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72268e96-275c-4daf-8690-0f9c127762ce"
            }
          ]
        },
        {
          "id": "5ea90c43-b839-4eee-8366-8df4403d4521",
          "name": "adminUpdateUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=AdminUpdateUserAttributes?UserAttributes=UserAttributes&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the specified user's attributes, including developer attributes, as an\n            administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdf1c8fc-d8bd-4459-aea3-10f36a13b692"
            }
          ]
        },
        {
          "id": "dc4ae878-b558-4cdc-8463-5a3a516de2b2",
          "name": "adminUserGlobalSignOut",
          "request": {
            "url": "http://example.com/api/?Action=AdminUserGlobalSignOut?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Signs out users from all devices, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5db94e60-4c1c-43e9-a4e7-a4ba0f6a7567"
            }
          ]
        },
        {
          "id": "cc9ee8ad-6cc0-4ebd-8e7d-058a433429d1",
          "name": "createUserImportJob",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserImportJob?CloudWatchLogsRoleArn=CloudWatchLogsRoleArn&JobName=JobName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the user import job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1944e4e5-60a2-4423-9560-4ab8129685e4"
            }
          ]
        },
        {
          "id": "1abf59fa-ca28-4c22-b125-68579a44d0de",
          "name": "createUserPool",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPool?AdminCreateUserConfig=AdminCreateUserConfig&AliasAttributes=AliasAttributes&AutoVerifiedAttributes=AutoVerifiedAttributes&DeviceConfiguration=DeviceConfiguration&EmailConfiguration=EmailConfiguration&EmailVerificationMessage=EmailVerificationMessage&EmailVerificationSubject=EmailVerificationSubject&LambdaConfig=LambdaConfig&MfaConfiguration=MfaConfiguration&Policies=Policies&PoolName=PoolName&Schema=Schema&SmsAuthenticationMessage=SmsAuthenticationMessage&SmsConfiguration=SmsConfiguration&SmsVerificationMessage=SmsVerificationMessage&UserPoolTags=UserPoolTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Amazon Cognito user pool and sets the password policy for the\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23cf568f-4ae5-453a-a04c-f41a8c39e580"
            }
          ]
        },
        {
          "id": "95a648cb-64f8-45fd-b96f-c47c934d6f91",
          "name": "createUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=CreateUserPoolClient?ClientName=ClientName&ExplicitAuthFlows=ExplicitAuthFlows&GenerateSecret=GenerateSecret&ReadAttributes=ReadAttributes&RefreshTokenValidity=RefreshTokenValidity&UserPoolId=UserPoolId&WriteAttributes=WriteAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d3093c91-ca1e-4e15-b91a-f07ea9983a67"
            }
          ]
        },
        {
          "id": "7cbb7473-f36c-4bcc-9069-57649f1db89a",
          "name": "deleteUser",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUser?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a user to delete one's self."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12655d6c-e480-471e-a872-5b4e2df6bc98"
            }
          ]
        },
        {
          "id": "0fad239d-e597-45e9-b626-f47764689546",
          "name": "deleteUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserAttributes?AccessToken=AccessToken&UserAttributeNames=UserAttributeNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the attributes for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90543e85-70cf-4c70-99cc-9808909cf4c1"
            }
          ]
        },
        {
          "id": "c37e9f12-826e-4009-8ef0-8cc6db800475",
          "name": "deleteUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified Amazon Cognito user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4af20f1c-a3c4-45ed-b6ad-42f4ec55fdd1"
            }
          ]
        },
        {
          "id": "4ca4cfc1-6fbd-4c29-b927-a7fd11ddaf4a",
          "name": "deleteUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DeleteUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the developer to delete the user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdfa54f5-62af-4169-a89c-ff99fd059832"
            }
          ]
        },
        {
          "id": "b61dc2c7-f988-4db9-a6b9-8ab6726fdfdd",
          "name": "describeUserImportJob",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserImportJob?JobId=JobId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the user import job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7317bba-c8d3-4b24-aa49-9ed4d3a9ce71"
            }
          ]
        },
        {
          "id": "36af63f7-b2ca-4ecd-9643-560f869668ba",
          "name": "describeUserPool",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPool?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the configuration information and metadata of the specified user\n            pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7acd9cd-f8ad-4025-946c-4c7582a51bf5"
            }
          ]
        },
        {
          "id": "e44d2a4a-57fc-4ff0-949b-14ecbf2d68f6",
          "name": "describeUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUserPoolClient?ClientId=ClientId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Client method for returning the configuration information and metadata of the\n            specified user pool client."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b43be0e6-80b7-4202-aec5-19139c866319"
            }
          ]
        },
        {
          "id": "8a147ac7-91a6-4b4a-8129-ede98da3874c",
          "name": "getDevice",
          "request": {
            "url": "http://example.com/api/?Action=GetDevice?AccessToken=AccessToken&DeviceKey=DeviceKey",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d10b2d2-ce48-4dfd-85fd-d35aa77d6af7"
            }
          ]
        },
        {
          "id": "fac9e085-6a4d-4a4b-ad22-af61a7aa1a6e",
          "name": "getUser",
          "request": {
            "url": "http://example.com/api/?Action=GetUser?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the user attributes and metadata for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1716ee02-06e8-449e-b6e2-b7ed0248f073"
            }
          ]
        },
        {
          "id": "67c3a696-f627-42e8-b56f-b91a0a4c3960",
          "name": "listUserImportJobs",
          "request": {
            "url": "http://example.com/api/?Action=ListUserImportJobs?MaxResults=MaxResults&PaginationToken=PaginationToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the user import jobs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04ec4fbe-2336-4f0a-b0a2-2bdbc7037e7e"
            }
          ]
        },
        {
          "id": "7ba62e37-0711-4c9d-908b-6664c01d8e8f",
          "name": "listUsers",
          "request": {
            "url": "http://example.com/api/?Action=ListUsers?AttributesToGet=AttributesToGet&Filter=Filter&Limit=Limit&PaginationToken=PaginationToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the users in the Amazon Cognito user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb4df62a-5466-4c61-be78-70e8a5211240"
            }
          ]
        },
        {
          "id": "94172926-3281-4702-ba53-a1162a91cfa5",
          "name": "listUsersInGroup",
          "request": {
            "url": "http://example.com/api/?Action=ListUsersInGroup?GroupName=GroupName&Limit=Limit&NextToken=NextToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the users in the specified group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8447adb5-3439-4a50-af61-aae180e31e8c"
            }
          ]
        },
        {
          "id": "1d09acde-3b5a-404d-bdf1-1405ba42d35a",
          "name": "setUserSettings",
          "request": {
            "url": "http://example.com/api/?Action=SetUserSettings?AccessToken=AccessToken&MFAOptions=MFAOptions",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the user settings like multi-factor authentication (MFA)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99f97aa6-0cad-418d-82cf-26fae8d7c79e"
            }
          ]
        },
        {
          "id": "46f7231e-08d1-4bcb-91a8-70273f8637c1",
          "name": "startUserImportJob",
          "request": {
            "url": "http://example.com/api/?Action=StartUserImportJob?JobId=JobId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts the user import."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05dfd544-7227-42ae-b567-c116bcd3035e"
            }
          ]
        },
        {
          "id": "1831467b-f40e-4f00-8dbd-bce23137f1b4",
          "name": "stopUserImportJob",
          "request": {
            "url": "http://example.com/api/?Action=StopUserImportJob?JobId=JobId&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Stops the user import job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09e8bb5f-aaa8-4e10-a176-bbb6f1f97298"
            }
          ]
        },
        {
          "id": "dc373aa4-76b5-4fe6-9610-1b6c917e8c3f",
          "name": "updateUserAttributes",
          "request": {
            "url": "http://example.com/api/?Action=UpdateUserAttributes?AccessToken=AccessToken&UserAttributes=UserAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a user to update a specific attribute (one at a time)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "871a0b45-be28-461f-9046-7aa0ad6ca57b"
            }
          ]
        },
        {
          "id": "6bef61e6-8097-48ce-8fd1-7a14ec86dd67",
          "name": "updateUserPool",
          "request": {
            "url": "http://example.com/api/?Action=UpdateUserPool?AdminCreateUserConfig=AdminCreateUserConfig&AutoVerifiedAttributes=AutoVerifiedAttributes&DeviceConfiguration=DeviceConfiguration&EmailConfiguration=EmailConfiguration&EmailVerificationMessage=EmailVerificationMessage&EmailVerificationSubject=EmailVerificationSubject&LambdaConfig=LambdaConfig&MfaConfiguration=MfaConfiguration&Policies=Policies&SmsAuthenticationMessage=SmsAuthenticationMessage&SmsConfiguration=SmsConfiguration&SmsVerificationMessage=SmsVerificationMessage&UserPoolId=UserPoolId&UserPoolTags=UserPoolTags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the specified user pool with the specified attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8245afdd-9e7b-4647-97f4-9fd15d9e2070"
            }
          ]
        },
        {
          "id": "b05dc116-bd17-4cd7-8b1c-2391c7fbfe68",
          "name": "updateUserPoolClient",
          "request": {
            "url": "http://example.com/api/?Action=UpdateUserPoolClient?ClientId=ClientId&ClientName=ClientName&ExplicitAuthFlows=ExplicitAuthFlows&ReadAttributes=ReadAttributes&RefreshTokenValidity=RefreshTokenValidity&UserPoolId=UserPoolId&WriteAttributes=WriteAttributes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows the developer to update the specified user pool client and password\n            policy."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ead4c4c3-c9f3-4d6e-be9d-78b719a846e2"
            }
          ]
        },
        {
          "id": "e2b9c0cf-6ba8-4087-94b7-23995956ba44",
          "name": "verifyUserAttribute",
          "request": {
            "url": "http://example.com/api/?Action=VerifyUserAttribute?AccessToken=AccessToken&AttributeName=AttributeName&Code=Code",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Verifies the specified user attributes in the user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9cc5ec56-eef7-4e2c-aea0-25af6fc4e1f8"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Up",
      "item": [
        {
          "id": "74a95452-cbae-4f06-a360-3963c79c3eae",
          "name": "adminConfirmSignUp",
          "request": {
            "url": "http://example.com/api/?Action=AdminConfirmSignUp?Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms user registration as an admin without using a confirmation code."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0550cc83-4b74-460a-b078-a40ab10011a9"
            }
          ]
        },
        {
          "id": "fc4b1609-792a-4ef4-8b1a-d039848000d5",
          "name": "signUp",
          "request": {
            "url": "http://example.com/api/?Action=SignUp?ClientId=ClientId&Password=Password&SecretHash=SecretHash&UserAttributes=UserAttributes&Username=Username&ValidationData=ValidationData",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers the user in the specified user pool and creates a user name, password,\n            and user attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85c5705c-791e-4c56-902a-06574d88b21b"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "8564c325-cab4-48a8-ba38-79e43f832161",
          "name": "adminForgetDevice",
          "request": {
            "url": "http://example.com/api/?Action=AdminForgetDevice?DeviceKey=DeviceKey&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forgets the device, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ad643777-cb99-4393-9db3-d9146f36f742"
            }
          ]
        },
        {
          "id": "9ed651f0-912a-4581-9743-15e021c32a2f",
          "name": "confirmDevice",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmDevice?AccessToken=AccessToken&DeviceKey=DeviceKey&DeviceName=DeviceName&DeviceSecretVerifierConfig=DeviceSecretVerifierConfig",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms tracking of the device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5856ab7e-1d78-49ac-afbb-5eb9399ed9c4"
            }
          ]
        },
        {
          "id": "cdc78ba0-5c04-4e0c-acf8-93c4662cb4b9",
          "name": "forgetDevice",
          "request": {
            "url": "http://example.com/api/?Action=ForgetDevice?AccessToken=AccessToken&DeviceKey=DeviceKey",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Forgets the specified device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "082265da-30b5-4b72-b158-6ae78081da50"
            }
          ]
        },
        {
          "id": "5775a95e-8cd4-48a7-8dc0-c64a8dd652aa",
          "name": "listDevices",
          "request": {
            "url": "http://example.com/api/?Action=ListDevices?AccessToken=AccessToken&Limit=Limit&PaginationToken=PaginationToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the devices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b2fbecb-a9fc-4bc0-ab36-8f757f9cc61d"
            }
          ]
        },
        {
          "id": "5d11cfb2-81ea-4e7f-b6a1-7f7f524bc348",
          "name": "updateDeviceStatus",
          "request": {
            "url": "http://example.com/api/?Action=UpdateDeviceStatus?AccessToken=AccessToken&DeviceKey=DeviceKey&DeviceRememberedStatus=DeviceRememberedStatus",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the device status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88989ed8-4740-44b5-8827-3426d2d0086d"
            }
          ]
        },
        {
          "id": "23ca525c-bcc3-4db2-b403-9fef80f50d10",
          "name": "registerDevice",
          "request": {
            "url": "http://example.com/api/?Action=RegisterDevice?IdentityId=IdentityId&IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a device to receive push sync notifications."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eaedd734-cc11-4ece-8eb2-4ecc77f8b3fb"
            }
          ]
        }
      ]
    },
    {
      "name": "http://laneworks.net/api-stack/pull/pull-amazon-cognito-sync.php",
      "item": [
        {
          "id": "857cc391-f548-460a-ae9f-e8a431cc5917",
          "name": "adminGetDevice",
          "request": {
            "url": "http://example.com/api/?Action=AdminGetDevice?DeviceKey=DeviceKey&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the device, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38b1bc7b-0302-4781-9630-8e0b3e36b913"
            }
          ]
        },
        {
          "id": "90904ead-072f-444c-9546-46baf7ac8dae",
          "name": "adminListDevices",
          "request": {
            "url": "http://example.com/api/?Action=AdminListDevices?Limit=Limit&PaginationToken=PaginationToken&Username=Username&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists devices, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2ff235b-2adc-4a76-8477-82e7b36ba62c"
            }
          ]
        }
      ]
    },
    {
      "name": "Authnetication",
      "item": [
        {
          "id": "486b4b95-ede6-4cb3-8546-0ce13943f087",
          "name": "adminInitiateAuth",
          "request": {
            "url": "http://example.com/api/?Action=AdminInitiateAuth?AuthFlow=AuthFlow&AuthParameters=AuthParameters&ClientId=ClientId&ClientMetadata=ClientMetadata&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates the authentication flow, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "20dabb85-b333-473d-bfb7-de89489116d4"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication Challenge",
      "item": [
        {
          "id": "4dcc5e25-39ed-48ae-9a58-29ffab495f30",
          "name": "adminRespondToAuthChallenge",
          "request": {
            "url": "http://example.com/api/?Action=AdminRespondToAuthChallenge?ChallengeName=ChallengeName&ChallengeResponses=ChallengeResponses&ClientId=ClientId&Session=Session&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Responds to an authentication challenge, as an administrator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "820475cf-25a8-4072-820d-098eeaa2e2e0"
            }
          ]
        }
      ]
    },
    {
      "name": "Password",
      "item": [
        {
          "id": "df1cb517-8caf-40ab-bd31-21205edeeea7",
          "name": "changePassword",
          "request": {
            "url": "http://example.com/api/?Action=ChangePassword?AccessToken=AccessToken&PreviousPassword=PreviousPassword&ProposedPassword=ProposedPassword",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Changes the password for a specified user in a user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a2355d8b-f40b-4452-a225-afd079bcd94c"
            }
          ]
        }
      ]
    },
    {
      "name": "Passwords",
      "item": [
        {
          "id": "18cef0b1-afb9-48c3-8198-a38c99d38cd9",
          "name": "confirmForgotPassword",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmForgotPassword?ClientId=ClientId&ConfirmationCode=ConfirmationCode&Password=Password&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows a user to enter a code provided when they reset their password to update\n            their password."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b598b5f-f85b-45ee-9720-ec3eb159f70e"
            }
          ]
        },
        {
          "id": "e4abb0d8-8e39-4b6e-a5fd-0cb0413ac868",
          "name": "forgotPassword",
          "request": {
            "url": "http://example.com/api/?Action=ForgotPassword?ClientId=ClientId&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the password for the specified client ID or username."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6bdd8404-36bf-47a2-8ce3-c8a984ed2bcb"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Ups",
      "item": [
        {
          "id": "4d10c3a3-d30f-4496-bcdb-1addb18366c9",
          "name": "confirmSignUp",
          "request": {
            "url": "http://example.com/api/?Action=ConfirmSignUp?ClientId=ClientId&ConfirmationCode=ConfirmationCode&ForceAliasCreation=ForceAliasCreation&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms registration of a user and handles the existing alias from a previous\n            user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40016bad-5b10-4d4c-987d-ca5a5d0cbd2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Groups",
      "item": [
        {
          "id": "2222fa11-0d67-4745-b384-3f3d848ec3e6",
          "name": "createGroup",
          "request": {
            "url": "http://example.com/api/?Action=CreateGroup?Description=Description&GroupName=GroupName&Precedence=Precedence&RoleArn=RoleArn&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new group in the specified user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "519715e9-5ddf-475c-9bd2-a91bda1cdc8e"
            }
          ]
        },
        {
          "id": "7b194ad6-cd77-4930-8d3e-418b4133423b",
          "name": "deleteGroup",
          "request": {
            "url": "http://example.com/api/?Action=DeleteGroup?GroupName=GroupName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2653c3f9-9af7-45e2-afb5-94a794bac75f"
            }
          ]
        },
        {
          "id": "9cafc771-2c12-4a66-b43e-73c794ec6664",
          "name": "getGroup",
          "request": {
            "url": "http://example.com/api/?Action=GetGroup?GroupName=GroupName&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a group."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e16812c-b6b6-422f-b30c-d15c027fe1f2"
            }
          ]
        },
        {
          "id": "7ef4f039-5e6a-49e5-9c63-e0b3bffc71de",
          "name": "listGroups",
          "request": {
            "url": "http://example.com/api/?Action=ListGroups?Limit=Limit&NextToken=NextToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the groups associated with a user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0639d4f-b41d-42bc-9ec6-ea17bff8fea4"
            }
          ]
        },
        {
          "id": "b9a5eca1-ef88-4390-bd41-6517e055021f",
          "name": "updateGroup",
          "request": {
            "url": "http://example.com/api/?Action=UpdateGroup?Description=Description&GroupName=GroupName&Precedence=Precedence&RoleArn=RoleArn&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the specified group with the specified attributes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2abca271-43f2-47f1-ba99-7b41c424e02a"
            }
          ]
        }
      ]
    },
    {
      "name": "CSV Header",
      "item": [
        {
          "id": "f502bd71-b598-43a4-b737-adabe88991b3",
          "name": "getCSVHeader",
          "request": {
            "url": "http://example.com/api/?Action=GetCSVHeader?UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the header information for the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0807df2d-77ae-4077-8f20-c98bc859cab8"
            }
          ]
        }
      ]
    },
    {
      "name": "Verification Codes",
      "item": [
        {
          "id": "7e2e6926-9d28-4442-831e-229b21ae416e",
          "name": "getUserAttributeVerificationCode",
          "request": {
            "url": "http://example.com/api/?Action=GetUserAttributeVerificationCode?AccessToken=AccessToken&AttributeName=AttributeName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the user attribute verification code for the specified attribute\n            name."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f565c65-b789-4788-872b-a873a4a81355"
            }
          ]
        }
      ]
    },
    {
      "name": "Sign Out",
      "item": [
        {
          "id": "ad5a7c49-3291-47d9-9fa7-c85ddf7dac3b",
          "name": "globalSignOut",
          "request": {
            "url": "http://example.com/api/?Action=GlobalSignOut?AccessToken=AccessToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Signs out users from all devices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e86d508-6e61-4b3e-b097-2a406c169985"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication",
      "item": [
        {
          "id": "753a2a0e-0309-4f47-a5ae-a2bde105680a",
          "name": "initiateAuth",
          "request": {
            "url": "http://example.com/api/?Action=InitiateAuth?AuthFlow=AuthFlow&AuthParameters=AuthParameters&ClientId=ClientId&ClientMetadata=ClientMetadata",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates the authentication flow."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef0d40b0-093d-4ac1-ac1e-05a075762cc3"
            }
          ]
        }
      ]
    },
    {
      "name": "user Pool Clients",
      "item": [
        {
          "id": "d213dfb6-7eaa-409d-8a2c-f726a529cdbe",
          "name": "listUserPoolClients",
          "request": {
            "url": "http://example.com/api/?Action=ListUserPoolClients?MaxResults=MaxResults&NextToken=NextToken&UserPoolId=UserPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the clients that have been created for the specified user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3592b90c-c27a-4997-ae4c-208fdb069ead"
            }
          ]
        }
      ]
    },
    {
      "name": "user Pools",
      "item": [
        {
          "id": "7c798cff-6634-4810-b5d0-a31e9cd0e4ee",
          "name": "listUserPools",
          "request": {
            "url": "http://example.com/api/?Action=ListUserPools?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the user pools associated with an AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2fae14e-1a12-4287-9dd0-20b7add4c30a"
            }
          ]
        }
      ]
    },
    {
      "name": "Confirmation Code",
      "item": [
        {
          "id": "1bef43f5-eff6-438a-8464-35531bd0a0e7",
          "name": "resendConfirmationCode",
          "request": {
            "url": "http://example.com/api/?Action=ResendConfirmationCode?ClientId=ClientId&SecretHash=SecretHash&Username=Username",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resends the confirmation (for confirmation of registration) to a specific user in\n            the user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4e4c333-50ea-4b9d-8cbb-cd135de7cc81"
            }
          ]
        }
      ]
    },
    {
      "name": "Authentication Challenges",
      "item": [
        {
          "id": "9e366277-2c1c-44e4-827a-104437c66fc0",
          "name": "respondToAuthChallenge",
          "request": {
            "url": "http://example.com/api/?Action=RespondToAuthChallenge?ChallengeName=ChallengeName&ChallengeResponses=ChallengeResponses&ClientId=ClientId&Session=Session",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Responds to the authentication challenge."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c48d4f03-61f2-4472-b3a6-227b729bc154"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity Pool",
      "item": [
        {
          "id": "86c6ff42-6a5e-4723-8789-fad764e64827",
          "name": "createIdentityPool",
          "request": {
            "url": "http://example.com/api/?Action=CreateIdentityPool?AllowUnauthenticatedIdentities=AllowUnauthenticatedIdentities&CognitoIdentityProviders=CognitoIdentityProviders&DeveloperProviderName=DeveloperProviderName&IdentityPoolName=IdentityPoolName&OpenIdConnectProviderARNs=OpenIdConnectProviderARNs&SamlProviderARNs=SamlProviderARNs&SupportedLoginProviders=SupportedLoginProviders",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new identity pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6676d2c1-aee7-4982-82bb-b820d4becb56"
            }
          ]
        },
        {
          "id": "3fd1edec-2fc6-4849-a0f1-8d78a1c0866b",
          "name": "deleteIdentityPool",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentityPool?IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b49f53eb-def7-47b2-bd45-45a78eed2f98"
            }
          ]
        },
        {
          "id": "68b18534-ad37-4b6b-937e-b1c5ba9eb978",
          "name": "describeIdentityPool",
          "request": {
            "url": "http://example.com/api/?Action=DescribeIdentityPool?IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets details about a particular identity pool, including the pool name, ID\n         description, creation date, and current number of users."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f483569-f39c-44cb-baf8-7b0875d0c2c5"
            }
          ]
        },
        {
          "id": "6f90045d-75d9-4714-91b9-e7dbcd7c1b4e",
          "name": "listIdentityPools",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentityPools?MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the Cognito identity pools registered for your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a47b3a1b-ca6f-40a9-8b1d-7412b0ab17fb"
            }
          ]
        },
        {
          "id": "21a24937-94d6-4652-87c5-d17ed1f6b71f",
          "name": "setIdentityPoolRoles",
          "request": {
            "url": "http://example.com/api/?Action=SetIdentityPoolRoles?IdentityPoolId=IdentityPoolId&RoleMappings=RoleMappings&Roles=Roles",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Sets the roles for an identity pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "290b2d37-71b5-41ad-9b32-bad37d7b84f1"
            }
          ]
        },
        {
          "id": "07be14ee-c196-466b-a1bd-77ef879da869",
          "name": "updateIdentityPool",
          "request": {
            "url": "http://example.com/api/?Action=UpdateIdentityPool?AllowUnauthenticatedIdentities=AllowUnauthenticatedIdentities&CognitoIdentityProviders=CognitoIdentityProviders&DeveloperProviderName=DeveloperProviderName&IdentityPoolId=IdentityPoolId&IdentityPoolName=IdentityPoolName&OpenIdConnectProviderARNs=OpenIdConnectProviderARNs&SamlProviderARNs=SamlProviderARNs&SupportedLoginProviders=SupportedLoginProviders",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a user pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "361bb5ee-32c9-4d00-9650-3511bb2e6a16"
            }
          ]
        }
      ]
    },
    {
      "name": "Identities",
      "item": [
        {
          "id": "4b9793f6-6587-45e8-8f9b-c43e1841eb64",
          "name": "deleteIdentities",
          "request": {
            "url": "http://example.com/api/?Action=DeleteIdentities?IdentityIdsToDelete=IdentityIdsToDelete",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes identities from an identity pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b8f725f-b362-43af-88a4-15a719f77750"
            }
          ]
        },
        {
          "id": "59dde315-600f-4144-8e61-3ab11d17a44f",
          "name": "describeIdentity",
          "request": {
            "url": "http://example.com/api/?Action=DescribeIdentity?IdentityId=IdentityId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metadata related to the given identity, including when the identity was\n         created and any associated linked logins."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "655623d2-037f-43b7-bb26-423136626e94"
            }
          ]
        },
        {
          "id": "ea915aaf-cbd3-4dab-8080-76cfa71c7c97",
          "name": "getCredentialsForIdentity",
          "request": {
            "url": "http://example.com/api/?Action=GetCredentialsForIdentity?CustomRoleArn=CustomRoleArn&IdentityId=IdentityId&Logins=Logins",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns credentials for the provided identity ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52008e72-16a4-4fa4-ac03-8deb35c122e1"
            }
          ]
        },
        {
          "id": "aa04e9ad-2e34-4a99-b6b7-69c1a48d84bd",
          "name": "getId",
          "request": {
            "url": "http://example.com/api/?Action=GetId?AccountId=AccountId&IdentityPoolId=IdentityPoolId&Logins=Logins",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generates (or retrieves) a Cognito ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af03e1ed-79ff-45ae-983f-90554b921762"
            }
          ]
        },
        {
          "id": "cca742eb-3edf-4739-8cc6-acb8027456d4",
          "name": "listIdentities",
          "request": {
            "url": "http://example.com/api/?Action=ListIdentities?HideDisabled=HideDisabled&IdentityPoolId=IdentityPoolId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the identities in a pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f1c53cb-0983-4de4-b241-a8d868805f93"
            }
          ]
        },
        {
          "id": "f7b00291-a116-40e5-b474-f1c46a6b0c71",
          "name": "unlinkIdentity",
          "request": {
            "url": "http://example.com/api/?Action=UnlinkIdentity?IdentityId=IdentityId&Logins=Logins&LoginsToRemove=LoginsToRemove",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Unlinks a federated identity from an existing account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a86c3d2-c718-493c-9acc-249a3d8d1d41"
            }
          ]
        }
      ]
    },
    {
      "name": "Identity Pool Roles",
      "item": [
        {
          "id": "a2bad416-8252-4a10-b7d6-247b56b3dd1f",
          "name": "getIdentityPoolRoles",
          "request": {
            "url": "http://example.com/api/?Action=GetIdentityPoolRoles?IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the roles for an identity pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a8f4f5f0-dea7-4526-946f-404ae3ce13a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Open ID Token",
      "item": [
        {
          "id": "77401700-df0c-48cf-a7ce-2b3e39c031be",
          "name": "getOpenIdToken",
          "request": {
            "url": "http://example.com/api/?Action=GetOpenIdToken?IdentityId=IdentityId&Logins=Logins",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets an OpenID token, using a known Cognito ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b4808ec-ba80-44a1-9812-abcebfc50fba"
            }
          ]
        }
      ]
    },
    {
      "name": "Open ID Token for Developer Identities",
      "item": [
        {
          "id": "17524c25-d56c-47c0-aab7-32c2755a4f02",
          "name": "getOpenIdTokenForDeveloperIdentity",
          "request": {
            "url": "http://example.com/api/?Action=GetOpenIdTokenForDeveloperIdentity?IdentityId=IdentityId&IdentityPoolId=IdentityPoolId&Logins=Logins&TokenDuration=TokenDuration",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Registers (or retrieves) a Cognito IdentityId and an OpenID Connect\n         token for a user authenticated by your backend authentication process."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13f31add-8c45-46f8-b8ef-4c3aac248a80"
            }
          ]
        }
      ]
    },
    {
      "name": "Developer Identities",
      "item": [
        {
          "id": "aaadb3ad-0311-4c42-a246-7a8ffdbc063e",
          "name": "lookupDeveloperIdentity",
          "request": {
            "url": "http://example.com/api/?Action=LookupDeveloperIdentity?DeveloperUserIdentifier=DeveloperUserIdentifier&IdentityId=IdentityId&IdentityPoolId=IdentityPoolId&MaxResults=MaxResults&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves the IdentityID associated with a\n            DeveloperUserIdentifier or the list of\n         DeveloperUserIdentifiers associated with an IdentityId for an\n         existing identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b73d65a2-6453-4007-aafe-f6d8d59f2031"
            }
          ]
        },
        {
          "id": "fafb7f94-bc19-4a19-8146-dda8d7202664",
          "name": "mergeDeveloperIdentities",
          "request": {
            "url": "http://example.com/api/?Action=MergeDeveloperIdentities?DestinationUserIdentifier=DestinationUserIdentifier&DeveloperProviderName=DeveloperProviderName&IdentityPoolId=IdentityPoolId&SourceUserIdentifier=SourceUserIdentifier",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Merges two users having different IdentityIds, existing in the same\n         identity pool, and identified by the same developer provider."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33a04534-baca-4e58-8944-4c2ba041097d"
            }
          ]
        },
        {
          "id": "10fa81f5-2a79-4abe-be84-5a2b46ce7c30",
          "name": "unlinkDeveloperIdentity",
          "request": {
            "url": "http://example.com/api/?Action=UnlinkDeveloperIdentity?DeveloperProviderName=DeveloperProviderName&DeveloperUserIdentifier=DeveloperUserIdentifier&IdentityId=IdentityId&IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Unlinks a DeveloperUserIdentifier from an existing identity."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c386f89-6ebd-4507-9cbf-a46c3eb29c83"
            }
          ]
        }
      ]
    },
    {
      "name": "Publish",
      "item": [
        {
          "id": "5fa46908-61a1-4ba5-9e45-ee1b0bb2be2d",
          "name": "bulkPublish",
          "request": {
            "url": "http://example.com/api/?Action=BulkPublish?IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a bulk publish of all existing datasets for an Identity Pool to the configured stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f66d118-9e31-4374-b19b-7660d44b6ca2"
            }
          ]
        },
        {
          "id": "e752385d-44e6-4698-9299-685ed8bedf0f",
          "name": "getBulkPublishDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetBulkPublishDetails?IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the status of the last BulkPublish operation for an identity pool."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9a689622-84ff-44b0-9c2f-4ac0c2b05d8f"
            }
          ]
        }
      ]
    },
    {
      "name": "Dataset",
      "item": [
        {
          "id": "5b15fe3f-d937-4f66-8fc9-f75e46f64967",
          "name": "deleteDataset",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDataset?DatasetName=DatasetName&IdentityId=IdentityId&IdentityPoolId=IdentityPoolId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specific da