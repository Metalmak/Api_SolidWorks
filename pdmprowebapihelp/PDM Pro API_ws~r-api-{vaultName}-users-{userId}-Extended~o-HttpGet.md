<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-users-{userId}-Extended~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/users/{userId}/Extended |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [User Resource Group](PDM%20Pro%20API_ws~g-d6cc2646-e51b-47df-b82a-a6bc98ec4601.html) : api/{vaultName}/users/{userId}/Extended (Get) |

Description

Get user info extended

Gets extended information about the specified user.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| userId | (URI parameter) User ID (required) | integer |
| UserInfo | (Body parameter) A UserInfo object that consists of:     UserName (string)     UserId (integer)    Member of UserInfoExtended model    (Response) A UserInfo object that consists of:     UserName (string)     UserId (integer)    Member of UserInfoExtended model | UserInfo |
| Email | (Body parameter) (Response) User email    Member of UserInfoExtended model | string |
| FullName | (Body parameter)    Member of UserInfoExtended model    (Response) User full name    Member of UserInfoExtended model | string |
| Initials | (Body parameter)    Member of UserInfoExtended model    (Response) User intials    Member of UserInfoExtended model | string |
| Phone | (Body parameter)    Member of UserInfoExtended model    (Response) User phone    Member of UserInfoExtended model | string |
| Cellphone | (Body parameter) Mobile phone    Member of UserInfoExtended model  (Response) User mobile phone    Member of UserInfoExtended model | string |

Response (application/json, text/json)

### Sample Data

```
{
  "UserInfo": {
    "UserName": "sample string 1",
    "UserId": 2
  },
  "Email": "sample string 1",
  "FullName": "sample string 2",
  "Initials": "sample string 3",
  "Phone": "sample string 4",
  "Cellphone": "sample string 5"
}
```

Response (application/xml, text/xml)

### Sample Data

```
<UserInfoExtended xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <Cellphone>sample string 5</Cellphone>
  <Email>sample string 1</Email>
  <FullName>sample string 2</FullName>
  <Initials>sample string 3</Initials>
  <Phone>sample string 4</Phone>
  <UserInfo>
    <UserId>2</UserId>
    <UserName>sample string 1</UserName>
  </UserInfo>
</UserInfoExtended>
```

See Also

[User Resource Group](PDM%20Pro%20API_ws~g-d6cc2646-e51b-47df-b82a-a6bc98ec4601.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)