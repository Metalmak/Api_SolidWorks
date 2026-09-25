<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-state-{transitionId}-HistoryComments~o-HttpPost.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Post | api/{vaultName}/state/{transitionId}/HistoryComments |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [State Transition Resource Group](PDM%20Pro%20API_ws~g-5d230f64-6d99-40c3-9dec-116da99c6424.html) : api/{vaultName}/state/{transitionId}/HistoryComments (Post) |

Description

Get transition comment history for multiple files

Gets the comment histories for specified files that undergo the specified transition.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| transitionId | (URI parameter) Transition ID (required) | integer |
| Comments | (Response) Array of history comments    Member of HistoryTransitionComment model | Collection of string |

Request (application/json, text/json)

Array of file IDs passed in the body parameter

### Sample Data

```
[
  1,
  2
]
```

Request (application/xml, text/xml)

Array of file IDs passed in a body parameter

### Sample Data

```
<ArrayOfint xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.microsoft.com/2003/10/Serialization/Arrays">
  <int>1</int>
  <int>2</int>
</ArrayOfint>
```

Request (application/x-www-form-urlencoded)

Response (application/json, text/json)

### Sample Data

```
{
  "Comments": [
    "sample string 1",
    "sample string 2"
  ]
}
```

Response (application/xml, text/xml)

### Sample Data

```
<HistoryTransitionComment xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <Comments xmlns:d2p1="http://schemas.microsoft.com/2003/10/Serialization/Arrays">
    <d2p1:string>sample string 1</d2p1:string>
    <d2p1:string>sample string 2</d2p1:string>
  </Comments>
</HistoryTransitionComment>
```

Remarks

This operation:

* takes a body parameter array of integers that are file IDs.* returns an array of HistoryTransitionComments.

See Also

[State Transition Resource Group](PDM%20Pro%20API_ws~g-5d230f64-6d99-40c3-9dec-116da99c6424.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)