<!-- source: pdmprowebapihelp/PDM Pro API_ws.html -->

PDM Pro API Web Service

PDM Pro API Web Service

Collapse All
Expand All

Description

The PDM Professional API Web Service consists of controllers and endpoints.

Authentication

|  |  |
| --- | --- |
| Post | [api/{vaultName}/authenticate](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-authenticate~o-HttpPost.html) Use for the authenticate to get authentication token   Authenticates the specified login for the specified vault and returns the authentication token and status. |

BOM

|  |  |
| --- | --- |
| Get | [api/{vaultName}/bom/{bomDocumentId}/{version}/{folderId}/named](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-bom-%7BbomDocumentId%7D-%7Bversion%7D-%7BfolderId%7D-named~o-HttpGet.html) Get named bom   Gets the specified BOM. |
| Get | [api/{vaultName}/bom/{bomTypeId}/{fileId}/{version}/{folderId}/computed?configId={configId}&latest={latest}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-bom-%7BbomTypeId%7D-%7BfileId%7D-%7Bversion%7D-%7BfolderId%7D-computed-configId%3D%7BconfigId%7D-latest%3D%7Blatest%7D~o-HttpGet.html) Get computed BOM   Gets the computed BOM. |
| Get | [api/{vaultName}/bom/{bomTypeId}/{fileId}/{version}/{folderId}/weldmentcutlist?configId={configId}&latest={latest}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-bom-%7BbomTypeId%7D-%7BfileId%7D-%7Bversion%7D-%7BfolderId%7D-weldmentcutlist-configId%3D%7BconfigId%7D-latest%3D%7Blatest%7D~o-HttpGet.html) Get computed BOM   Gets the weldment cut list BOM. |

Configuration

|  |  |
| --- | --- |
| Get | [api/configuration/vaults?vaultName={vaultName}](PDM%20Pro%20API_ws~r-api-configuration-vaults-vaultName%3D%7BvaultName%7D~o-HttpGet.html) Get all vaults from the config file   Gets all vaults from the vault configuration file. |

Data Card

|  |  |
| --- | --- |
| Get | [api/{vaultName}/files/{fileId}/{version}/datacard?folderId={folderId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-datacard-folderId%3D%7BfolderId%7D~o-HttpGet.html) Get file data card   Gets the data card for the specified file, file version, and vault. |
| Post | [api/{vaultName}/files/{fileId}/datacard](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-datacard~o-HttpPost.html) Save file data card   Saves the data card for the specified file and vault. |
| Get | [api/{vaultName}/folders/{folderId}/datacard](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D-datacard~o-HttpGet.html) Get folder data card   Gets the data card for the specified folder and vault. |

Default

|  |  |
| --- | --- |
| Get | [api/{uri}](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpGet.html) Uses the specified URI to get information. |
| Post | [api/{uri}](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpPost.html) Uses the specified URI to post information. |
| Put | [api/{uri}](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpPut.html) Uses the specified URI to save information. |
| Patch | [api/{uri}](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpPatch.html) Uses the specified URI to patch information. |
| Delete | [api/{uri}](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpDelete.html) Uses the specified URI to delete information. |

File

|  |  |
| --- | --- |
| Get | [api/{vaultName}/files/{fileId}/{version}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D~o-HttpGet.html) Get file info   Gets information about the specified file. |
| Get | [api/{vaultName}/files/{fileId}/{version}/ActiveConfig](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-ActiveConfig~o-HttpGet.html) Get active configuration   Gets the active configuration of the specified file. |
| Get | [api/{vaultName}/files/{fileId}/{version}/allreferences?configId={configId}&folderId={folderId}&includeSubParents={includeSubParents}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-allreferences-configId%3D%7BconfigId%7D-folderId%3D%7BfolderId%7D-includeSubParents%3D%7BincludeSubParents%7D~o-HttpGet.html) Get all file references   Gets the reference tree of the specified file. |
| Get | [api/{vaultName}/files/{fileId}/{version}/configurations](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-configurations~o-HttpGet.html) Get file configurations   Gets the configurations of the specified file. |
| Get | [api/{vaultName}/files/{fileId}/{version}/download](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-download~o-HttpGet.html) Get file   Gets the link to download a file. |
| Get | [api/{vaultName}/files/{fileId}/{version}/info](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-info~o-HttpGet.html) Get file info   Gets information about the specified file. |
| Get | [api/{vaultName}/files/{fileId}/{version}/info/extended](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-info-extended~o-HttpGet.html) Get file info extended   Gets extended file information. |
| Get | [api/{vaultName}/files/{fileId}/{version}/references?configId={configId}&folderId={folderId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-references-configId%3D%7BconfigId%7D-folderId%3D%7BfolderId%7D~o-HttpGet.html) Get file references   Gets the top level file references of the specified file. |
| Get | [api/{vaultName}/files/{fileId}/{version}/thumbnails](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-thumbnails~o-HttpGet.html) Get file thumbnail   Gets the link to download a file thumbnail. |
| Get | [api/{vaultName}/files/{fileId}/{version}/variables](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-variables~o-HttpGet.html) Get file variables   Gets the specified file's variables. |
| Get | [api/{vaultName}/files/{fileId}/{version}/whereused?configId={configId}&folderId={folderId}&anyVersion={anyVersion}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-whereused-configId%3D%7BconfigId%7D-folderId%3D%7BfolderId%7D-anyVersion%3D%7BanyVersion%7D~o-HttpGet.html) Get file where used   Gets the parents of the specified file. |
| Get | [api/{vaultName}/files/{fileId}/bominfo?folderId={folderId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-bominfo-folderId%3D%7BfolderId%7D~o-HttpGet.html) Get file BOM info   Gets the BOM information for the specified file. |
| Get | [api/{vaultName}/files/{fileId}/info?version={version}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-info-version%3D%7Bversion%7D~o-HttpGet.html) Get file info   Gets information about the specified file. |
| Get | [api/{vaultName}/files/{fileId}/transitions?version={version}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-transitions-version%3D%7Bversion%7D~o-HttpGet.html) Get file transitions   Gets the state transitions for the specified file. |
| Get | [api/{vaultName}/files/{fileId}/versions?folderId={folderId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-versions-folderId%3D%7BfolderId%7D~o-HttpGet.html) Get file version info   Gets the specified file's version information. |
| Delete | [api/{vaultName}/files/{fileId}?destroy={destroy}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-destroy%3D%7Bdestroy%7D~o-HttpDelete.html) Delete file   Deletes the specified file |
| Get | [api/{vaultName}/files/{fileId}?version={version}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-version%3D%7Bversion%7D~o-HttpGet.html) Get file info   Gets information about the specified file. |
| Post | [api/{vaultName}/files/buildtree/checkout](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-buildtree-checkout~o-HttpPost.html) Build checkout references tree   Gets the tree of references in the specified file's checkout. |
| Post | [api/{vaultName}/files/buildtree/undo](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-buildtree-undo~o-HttpPost.html) Build undo checkout references tree   Builds the reference tree to undo the checkout of the specified file. |
| Post | [api/{vaultName}/files/CheckOut](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-CheckOut~o-HttpPost.html) Lock file   Checks out the specified file. |
| Post | [api/{vaultName}/files/info](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-info~o-HttpPost.html) Get file info   Gets information about multiple files. |
| Post | [api/{vaultName}/files/UndoCheckOut](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-UndoCheckOut~o-HttpPost.html) Undo lock file   Unlocks the specified file. |

Folder

|  |  |
| --- | --- |
| Get | [api/{vaultName}/folders/{folderId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D~o-HttpGet.html) Get folder info   Gets information for the specified folder. |
| Get | [api/{vaultName}/folders/{folderId}/browse](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D-browse~o-HttpGet.html) Get browse folder   Gets the files and folders in the specified folder. |
| Get | [api/{vaultName}/folders/{folderId}/info](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D-info~o-HttpGet.html) Get folder info   Gets information for the specified folder. |
| Delete | [api/{vaultName}/folders/{folderId}?destroy={destroy}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D-destroy%3D%7Bdestroy%7D~o-HttpDelete.html) Delete folder   Deletes the specified folder. |
| Put | [api/{vaultName}/folders/{parentFolderId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BparentFolderId%7D~o-HttpPut.html) Add folder   Adds a folder to the specified folder. |
| Post | [api/{vaultName}/folders/info](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-info~o-HttpPost.html) Get folder info   Gets information about specified folders in the specified vault. |

Group

|  |  |
| --- | --- |
| Get | [api/{vaultName}/groups](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-groups~o-HttpGet.html) Get groups   Gets the groups in the specified vault. |
| Get | [api/{vaultName}/groups/{groupId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-groups-%7BgroupId%7D~o-HttpGet.html) Get group info   Gets information about the specified group. |
| Get | [api/{vaultName}/groups/{groupId}/info](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-groups-%7BgroupId%7D-info~o-HttpGet.html) Get group info   Gets information about the specified group. |
| Get | [api/{vaultName}/groups/all](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-groups-all~o-HttpGet.html) Get groups   Gets the groups in the specified vault. |

Notification

|  |  |
| --- | --- |
| Post | [api/{vaultName}/notifications](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-notifications~o-HttpPost.html) Send message   Sends the specified message. |
| Post | [api/{vaultName}/notifications/markRead](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-notifications-markRead~o-HttpPost.html) Mark message as read   Marks a notification as read. |
| Get | [api/{vaultName}/notifications?all={all}&pageNo={pageNo}&pageSize={pageSize}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-notifications-all%3D%7Ball%7D-pageNo%3D%7BpageNo%7D-pageSize%3D%7BpageSize%7D~o-HttpGet.html) Get user notifications   Gets the user notifications. |

Progress

|  |  |
| --- | --- |
| Get | [api/{vaultName}/progress/{guid}/result](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-progress-%7Bguid%7D-result~o-HttpGet.html) Get operation result   Gets the result of the specified operation. |
| Get | [api/{vaultName}/progress/{guid}/status](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-progress-%7Bguid%7D-status~o-HttpGet.html) Get operation status   Gets the status of the specified operation. |

Stage

|  |  |
| --- | --- |
| Get | [api/{vaultName}/changeset/create](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-changeset-create~o-HttpGet.html) Generate changesetId   Gets a changeset ID for the specified vault. |
| Put | [api/{vaultName}/checkin/{changesetId}/{overrideVersion}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-%7BchangesetId%7D-%7BoverrideVersion%7D~o-HttpPut.html) Check in files from the changeset   Checks in the specified changeset. |
| Put | [api/{vaultName}/checkin/addfiles/{changesetId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-addfiles-%7BchangesetId%7D~o-HttpPut.html) Upload files or document ids to changeset to the check in operation   Uploads files to the specified changeset for checkin. |
| Get | [api/{vaultName}/checkin/buildtree/{changesetId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-buildtree-%7BchangesetId%7D~o-HttpGet.html) Get references tree   Builds a reference tree of files that are uploaded to the specified changeset. |
| Put | [api/{vaultName}/files/{changesetId}/finishadd](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BchangesetId%7D-finishadd~o-HttpPut.html) Finish of add file operation. This method adds files from changeset to the vault.   Adds files in the specified changeset to the vault. |
| Put | [api/{vaultName}/files/{changesetId}/upload](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BchangesetId%7D-upload~o-HttpPut.html) Upload file to changeset to add files operations   Uploads a changeset. |

State Transition

|  |  |
| --- | --- |
| Get | [api/{vaultName}/state/{documentId}/{folderId}/{transitionId}/references](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BdocumentId%7D-%7BfolderId%7D-%7BtransitionId%7D-references~o-HttpGet.html) Get all references   Gets all references for the specified file and transition. |
| Get | [api/{vaultName}/state/{documentId}/transitions](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BdocumentId%7D-transitions~o-HttpGet.html) Get available transitions for single file   Gets the transitions available for the specified file. |
| Get | [api/{vaultName}/state/{transitionId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D~o-HttpGet.html) Get transition info   Gets information about the specified transition. |
| Post | [api/{vaultName}/state/{transitionId}/changestate?revoke={revoke}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-changestate-revoke%3D%7Brevoke%7D~o-HttpPost.html) Change state   Changes the state of the specified documents. |
| Post | [api/{vaultName}/state/{transitionId}/DynamicNotificationUsers](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-DynamicNotificationUsers~o-HttpPost.html) Get dynamic notification users   Gets the users to notify when the specified items undergo the specified transition. |
| Post | [api/{vaultName}/state/{transitionId}/HistoryComments](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-HistoryComments~o-HttpPost.html) Get transition comment history for multiple files   Gets the comment histories for specified files that undergo the specified transition. |
| Post | [api/{vaultName}/state/transitions](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-transitions~o-HttpPost.html) Get available transitions for multiple files   Gets the transitions available for multiple files. |

User

|  |  |
| --- | --- |
| Get | [api/{vaultName}/users](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users~o-HttpGet.html) Get users   Gets the users of the specified vault. |
| Get | [api/{vaultName}/users/{userId}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D~o-HttpGet.html) Get user info   Gets information about the specified user. |
| Get | [api/{vaultName}/users/{userId}/Extended](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Extended~o-HttpGet.html) Get user info extended   Gets extended information about the specified user. |
| Put | [api/{vaultName}/users/{userId}/Extended](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Extended~o-HttpPut.html) Set user info extended   Saves information about the specified user. |
| Get | [api/{vaultName}/users/{userId}/info](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-info~o-HttpGet.html) Get user info   Gets information about the specified user. |
| Get | [api/{vaultName}/users/{userId}/Picture](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Picture~o-HttpGet.html) Get user picture   Gets the picture of the specified user. |
| Put | [api/{vaultName}/users/{userId}/Picture](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Picture~o-HttpPut.html) Put user picture   Saves the picture of the specified user. |
| Delete | [api/{vaultName}/users/{userId}/Picture](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Picture~o-HttpDelete.html) Delete user picture   Deletes the picture of the specified user. |
| Get | [api/{vaultName}/users/all](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-all~o-HttpGet.html) Get users   Gets the users of the specified vault. |

Vault

|  |  |
| --- | --- |
| Get | [api/{vaultName}](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D~o-HttpGet.html) Get vault properties   Gets the properties of the specified vault. |
| Post | [api/{vaultName}/delete/computetree](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-delete-computetree~o-HttpPost.html) Delete compute tree   Deletes the specified items in the specified vault. |
| Get | [api/{vaultName}/info](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-info~o-HttpGet.html) Get vault properties   Gets the properties of the specified vault. |
| Get | [api/{vaultName}/search](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-search~o-HttpGet.html) Search vault   Gets objects in the specified vault. |
| Post | [api/{vaultName}/search](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-search~o-HttpPost.html) Search vault   Gets objects in the vault that contain the specified string. |

Version

|  |  |
| --- | --- |
| Get | [api/version/webapi](PDM%20Pro%20API_ws~r-api-version-webapi~o-HttpGet.html) Get version   Gets the version of this web application. |

Workflow

|  |  |
| --- | --- |
| Get | [api/{vaultName}/workflows](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-workflows~o-HttpGet.html) Get workflows   Gets the workflows in the specified vault. |
| Get | [api/{vaultName}/workflows/icons](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-workflows-icons~o-HttpGet.html) Get state icons   Gets the workflow state icons in the specified vault. |