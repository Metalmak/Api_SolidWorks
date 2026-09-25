<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-bom-{bomTypeId}-{fileId}-{version}-{folderId}-computed-configId={configId}-latest={latest}~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/bom/{bomTypeId}/{fileId}/{version}/{folderId}/computed?configId={configId}&latest={latest} |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [BOM Resource Group](PDM%20Pro%20API_ws~g-9660650f-529f-427a-9a5b-f094fa68a3c2.html) : api/{vaultName}/bom/{bomTypeId}/{fileId}/{version}/{folderId}/computed?configId={configId}&latest={latest} (Get) |

Description

Get computed BOM

Gets the computed BOM.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required in URI) | string |
| bomTypeId | (URI parameter) BOM type ID (required in URI) | integer |
| fileId | (URI parameter) File ID (required in URI) | integer |
| version | (URI parameter) Version (required in URI) | integer |
| folderId | (URI parameter) Folder ID (required in URI) | integer |
| configId | (URI parameter) Configuration ID (default is -1) | integer |
| latest | (URI parameter) Whether the latest version (default is false) | boolean |
| Columns | (Response) Array of BOMColumns; each BOMColumn consists of:   * ColumnNo (integer)* ColumnName (string)   Member of ComputedBOM model | Collection of BOMColumn |
| File | (Response) BOMRef consists of:   * File (BOMRow)* References (Collection of BOMRef)   Member of ComputedBOM model | BOMRef |

Response (application/json)

Response (text/json)

Response (application/xml)

Response (text/xml)

See Also

[BOM Resource Group](PDM%20Pro%20API_ws~g-9660650f-529f-427a-9a5b-f094fa68a3c2.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)