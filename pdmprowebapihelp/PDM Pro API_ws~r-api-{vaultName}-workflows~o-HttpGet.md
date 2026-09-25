<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-workflows~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/workflows |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Workflow Resource Group](PDM%20Pro%20API_ws~g-122bb1a3-edf9-40bb-8048-1bde9c77441c.html) : api/{vaultName}/workflows (Get) |

Description

Get workflows

Gets the workflows in the specified vault.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| Workflows | (Response) Array of Workflow objects; each Workflow consists of:     WorkflowId (integer)     WorkflowName (string)     States (array of StateInfo objects; each StateInfo consists of:        StateId (integer)        StateName (string)        IgnorePreviousPermissions (integer: 1 to ignore previous permission, 0 to not)     )    Member of WorkflowList model | Collection of Workflow |

Response (application/json, text/json)

### Sample Data

```
{
  "Workflows": [
    {
      "WorkflowId": 1,
      "WorkflowName": "sample string 2",
      "States": [
        {
          "StateId": 1,
          "StateName": "sample string 2",
          "IgnorePreviousPermissions": 3
        },
        {
          "StateId": 1,
          "StateName": "sample string 2",
          "IgnorePreviousPermissions": 3
        }
      ]
    },
    {
      "WorkflowId": 1,
      "WorkflowName": "sample string 2",
      "States": [
        {
          "StateId": 1,
          "StateName": "sample string 2",
          "IgnorePreviousPermissions": 3
        },
        {
          "StateId": 1,
          "StateName": "sample string 2",
          "IgnorePreviousPermissions": 3
        }
      ]
    }
  ]
}
```

Response (application/xml, text/xml)

### Sample Data

```
<WorkflowList xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <Workflows>
    <Workflow>
      <States>
        <StateInfo>
          <IgnorePreviousPermissions>3</IgnorePreviousPermissions>
          <StateId>1</StateId>
          <StateName>sample string 2</StateName>
        </StateInfo>
        <StateInfo>
          <IgnorePreviousPermissions>3</IgnorePreviousPermissions>
          <StateId>1</StateId>
          <StateName>sample string 2</StateName>
        </StateInfo>
      </States>
      <WorkflowId>1</WorkflowId>
      <WorkflowName>sample string 2</WorkflowName>
    </Workflow>
    <Workflow>
      <States>
        <StateInfo>
          <IgnorePreviousPermissions>3</IgnorePreviousPermissions>
          <StateId>1</StateId>
          <StateName>sample string 2</StateName>
        </StateInfo>
        <StateInfo>
          <IgnorePreviousPermissions>3</IgnorePreviousPermissions>
          <StateId>1</StateId>
          <StateName>sample string 2</StateName>
        </StateInfo>
      </States>
      <WorkflowId>1</WorkflowId>
      <WorkflowName>sample string 2</WorkflowName>
    </Workflow>
  </Workflows>
</WorkflowList>
```

See Also

[Workflow Resource Group](PDM%20Pro%20API_ws~g-122bb1a3-edf9-40bb-8048-1bde9c77441c.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)