<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-groups-{groupId}-info~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/groups/{groupId}/info |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Group Resource Group](PDM%20Pro%20API_ws~g-ce48d38f-320c-4422-a127-e5209c7e2b12.html) : api/{vaultName}/groups/{groupId}/info (Get) |

Description

Get group info

Gets information about the specified group.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| groupId | (URI and response parameter) Group ID (URI required)    Member of GroupInfo model | integer |
| GroupName | (Response) Group name    Member of GroupInfo model | string |

Response (application/json, text/json)

### Sample Data

```
{
  "GroupId": 1,
  "GroupName": "sample string 2"
}
```

Response (application/xml, text/xml)

### Sample Data

```
<GroupInfo xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <GroupId>1</GroupId>
  <GroupName>sample string 2</GroupName>
</GroupInfo>
```

See Also

[Group Resource Group](PDM%20Pro%20API_ws~g-ce48d38f-320c-4422-a127-e5209c7e2b12.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)