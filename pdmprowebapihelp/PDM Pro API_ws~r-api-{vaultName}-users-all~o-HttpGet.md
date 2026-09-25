<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-users-all~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/users/all |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [User Resource Group](PDM%20Pro%20API_ws~g-d6cc2646-e51b-47df-b82a-a6bc98ec4601.html) : api/{vaultName}/users/all (Get) |

Description

Get users

Gets the users of the specified vault.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| UserInfo | (Response) A UserInfo object that consists of:     UserName (string)     UserId (integer)    Member of UserInfoFull model | UserInfo |
| FullName | (Response) User name    Member of UserInfoFull model | string |
| Initials | (Response) User initials    Member of UserInfoFull model | string |

Response (application/json, text/json)

### Sample Data

```
[
  {
    "UserInfo": {
      "UserName": "sample string 1",
      "UserId": 2
    },
    "FullName": "sample string 1",
    "Initials": "sample string 2"
  },
  {
    "UserInfo": {
      "UserName": "sample string 1",
      "UserId": 2
    },
    "FullName": "sample string 1",
    "Initials": "sample string 2"
  }
]
```

Response (application/xml, text/xml)

### Sample Data

```
<ArrayOfUserInfoFull xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <UserInfoFull>
    <FullName>sample string 1</FullName>
    <Initials>sample string 2</Initials>
    <UserInfo>
      <UserId>2</UserId>
      <UserName>sample string 1</UserName>
    </UserInfo>
  </UserInfoFull>
  <UserInfoFull>
    <FullName>sample string 1</FullName>
    <Initials>sample string 2</Initials>
    <UserInfo>
      <UserId>2</UserId>
      <UserName>sample string 1</UserName>
    </UserInfo>
  </UserInfoFull>
</ArrayOfUserInfoFull>
```

See Also

[User Resource Group](PDM%20Pro%20API_ws~g-d6cc2646-e51b-47df-b82a-a6bc98ec4601.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)