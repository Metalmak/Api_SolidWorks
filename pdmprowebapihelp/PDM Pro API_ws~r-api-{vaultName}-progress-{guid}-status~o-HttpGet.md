<!-- source: pdmprowebapihelp/PDM Pro API_ws~r-api-{vaultName}-progress-{guid}-status~o-HttpGet.html -->

PDM Pro API Web Service

|  |  |
| --- | --- |
| Get | api/{vaultName}/progress/{guid}/status |

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) > [Progress Resource Group](PDM%20Pro%20API_ws~g-2279cdf6-53fe-4409-9acb-8511c5f37590.html) : api/{vaultName}/progress/{guid}/status (Get) |

Description

Get operation status

Gets the status of the specified operation.

Parameters

| Name | Description | Data Type |
| --- | --- | --- |
| vaultName | (URI parameter) Vault name (required) | string |
| guid | (URI parameter) Operation GUID (required) | string |
| Version | (Response) A Version model that consists of:   * Major (integer)* Minor (integer)* Build (integer)* Revision (integer)* MajorRevision (integer)* MinorRevision (integer)   Member of HttpResponseMessage model | Version |
| Content | (Response) Entity body and content headers    Member of HttpResponseMessage model | HttpContent |
| StatusCode | (Response) Status code; see <https://en.wikipedia.org/wiki/List_of_HTTP_status_codes>    Member of HttpResponseMessage model | HttpStatusCode |
| ReasonPhrase | (Response) Reason    Member of HttpResponseMessage model | string |
| Headers | (Response) Array of headers    Member of HttpResponseMessage model | Collection of Object |
| RequestMessage | (Response) An HttpRequestMessage object that consists of:     Version (Version model)     Content (HttpContent object consisting of Headers array)     Method (HttpMethod object consisting of Method string)     RequestUri (URI)     Headers (array of objects)     Properties (Dictionary of string [key] and Object [value]    Member of HttpResponseMessage model | HttpRequestMessage |
| IsSuccessStatusCode | (Response) True if successful, false if not    Member of HttpResponseMessage model | boolean |

See Also

[Progress Resource Group](PDM%20Pro%20API_ws~g-2279cdf6-53fe-4409-9acb-8511c5f37590.html)
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html)