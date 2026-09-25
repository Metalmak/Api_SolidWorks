<!-- source: pdmprowebapihelp/PDM Pro API_ws~g-d61f95b6-4b32-4c36-a0ec-956478ec12e0.html -->

PDM Pro API Web Service

State Transition Resource Group

Collapse All
Expand All

|  |
| --- |
| [PDM Pro API Web Service](PDM%20Pro%20API_ws.html) : State Transition Resource Group |

Description

Consists of APIs for working with states and transitions.

Operations

|  |  |
| --- | --- |
| Get | [api/{vaultName}/state/{documentId}/{folderId}/{transitionId}/references](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BdocumentId%7D-%7BfolderId%7D-%7BtransitionId%7D-references~o-HttpGet.html) GET: api/{vaultName}/state/{documentId}/{folderId}/{transitionId}/references Get all references   Gets all references for the specified file and transition. |
| Get | [api/{vaultName}/state/{documentId}/transitions](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BdocumentId%7D-transitions~o-HttpGet.html) GET: api/{vaultName}/state/{documentId}/transitions Get available transitions for single file   Gets the transitions available for the specified file. |
| Get | [api/{vaultName}/state/{transitionId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D~o-HttpGet.html) GET: api/{vaultName}/state/{transitionId} Get transition info   Gets information about the specified transition. |
| Post | [api/{vaultName}/state/{transitionId}/changestate?revoke={revoke}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-changestate-revoke%3D%7Brevoke%7D~o-HttpPost.html) POST: api/{vaultName}/state/{transitionId}/changestate Change state   Changes the state of the specified documents. |
| Post | [api/{vaultName}/state/{transitionId}/DynamicNotificationUsers](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-DynamicNotificationUsers~o-HttpPost.html) POST: api/{vaultName}/state/{transitionId}/DynamicNotificationUsers Get dynamic notification users   Gets the users to notify when the specified items undergo the specified transition. |
| Post | [api/{vaultName}/state/{transitionId}/HistoryComments](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-HistoryComments~o-HttpPost.html) POST: api/{vaultName}/state/{transitionId}/HistoryComments Get transition comment history for multiple files   Gets the comment histories for specified files that undergo the specified transition. |
| Post | [api/{vaultName}/state/transitions](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-transitions~o-HttpPost.html) POST: api/{vaultName}/state/transitions Get available transitions for multiple files   Gets the transitions available for multiple files. |

See Also

[PDM Pro API Web Service](PDM%20Pro%20API_ws.html)