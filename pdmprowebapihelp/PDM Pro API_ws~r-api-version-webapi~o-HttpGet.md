<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-version-webapi~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/version/webapi |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Version Resource Group](PDM%20Pro%20API_ws~g-5b4ebd33-009f-4dd6-9fea-90679aa8458a.html) : api/version/webapi (Get) |

Description

Get version

Gets the version of this web application.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| SwCompany | (Response) Company    Member of WebAPIVersionModel model | string |
| SWCopyright | (Response) Copyright    Member of WebAPIVersionModel model | string |
| ProdName | (Response) Product name    Member of WebAPIVersionModel model | string |
| ProdAppVersion | (Response) Product application version    Member of WebAPIVersionModel model | string |
| ProdFileVersion | (Response) Product file version    Member of WebAPIVersionModel model | string |

Response (application/json, text/json)

### Sample Data

```
{
  "SwCompany": "sample string 1",
  "SWCopyright": "sample string 2",
  "ProdName": "sample string 3",
  "ProdAppVersion": "sample string 4",
  "ProdFileVersion": "sample string 5"
}
```

Response (application/xml, text/xml)

### Sample Data

```
<WebAPIVersionModel xmlns:i="http://www.w3.org/2001/XMLSchema-instance" xmlns="http://schemas.datacontract.org/2004/07/SWPDM.Models">
  <ProdAppVersion>sample string 4</ProdAppVersion>
  <ProdFileVersion>sample string 5</ProdFileVersion>
  <ProdName>sample string 3</ProdName>
  <SWCopyright>sample string 2</SWCopyright>
  <SwCompany>sample string 1</SwCompany>
</WebAPIVersionModel>
```

See Also

[Version Resource Group](PDM%20Pro%20API_ws~g-5b4ebd33-009f-4dd6-9fea-90679aa8458a.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)