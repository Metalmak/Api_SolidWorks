<!-- source: pdmprowebapihelp/ReleaseNotes.html -->

![](images/collapse.gif)
![](images/expand.gif)
![](images/copycode.gif)
![](images/copycodeHighlight.gif)
![](images/drpdown.gif)
![](images/drpdown_orange.gif)

|  |
| --- |
|  |

|  |  |
| --- | --- |
| PDM Pro Web API Help |  |
| Release Notes |
|  | |

Glossary Item Box

This topic provides you with quick access to the enhancements in SOLIDWORKS PDM Professional Web API 2022.

#### Service Pack 0

##### New endpoints

###### [Authentication](PDM%20Pro%20API_ws~g-2606198f-8b8d-40b7-9a68-df2441b1fbf9.html)

* [api/{vaultName}/authenticate (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-authenticate~o-HttpPost.html)

###### [BOM](PDM%20Pro%20API_ws~g-a1c1f7bb-5344-4008-9dd3-69e3146801f7.html)

* [api/{vaultName}/bom/{bomDocumentId}/{version}/{folderId}/named (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-bom-%7BbomDocumentId%7D-%7Bversion%7D-%7BfolderId%7D-named~o-HttpGet.html)* [api/{vaultName}/bom/{bomTypeId}/{fileId}/{version}/{folderId}/computed?configId={configId}&latest={latest} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-bom-%7BbomTypeId%7D-%7BfileId%7D-%7Bversion%7D-%7BfolderId%7D-computed-configId%3D%7BconfigId%7D-latest%3D%7Blatest%7D~o-HttpGet.html)* [api/{vaultName}/bom/{bomTypeId}/{fileId}/{version}/{folderId}/weldmentcutlist?configId={configId}&latest={latest} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-bom-%7BbomTypeId%7D-%7BfileId%7D-%7Bversion%7D-%7BfolderId%7D-weldmentcutlist-configId%3D%7BconfigId%7D-latest%3D%7Blatest%7D~o-HttpGet.html)

###### [Configuration](PDM%20Pro%20API_ws~g-605d90c5-931d-46ef-b9fe-b26deac614b7.html)

* [api/configuration/vaults?vaultName={vaultName} (Get)](PDM%20Pro%20API_ws~r-api-configuration-vaults-vaultName%3D%7BvaultName%7D~o-HttpGet.html)

###### [Data Card](PDM%20Pro%20API_ws~g-5ccab900-17cd-44b2-9dc5-8cf0d8315ee6.html)

* [api/{vaultName}/files/{fileId}/{version}/datacard?folderId={folderId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-datacard-folderId%3D%7BfolderId%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/datacard (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-datacard~o-HttpPost.html)* [api/{vaultName}/folders/{folderId}/datacard (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D-datacard~o-HttpGet.html)

###### [Default](PDM%20Pro%20API_ws~g-ec3de890-9a9c-4ab1-9781-b5db1e047537.html)

* [api/{uri} (Get)](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpGet.html)* [api/{uri} (Post)](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpPost.html)* [api/{uri} (Put)](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpPut.html)* [api/{uri} (Patch)](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpPatch.html)* [api/{uri} (Delete)](PDM%20Pro%20API_ws~r-api-%7Buri%7D~o-HttpDelete.html)

###### [File](PDM%20Pro%20API_ws~g-c98f0c35-a34d-4136-b9d9-0017d3189da7.html)

* [api/{vaultName}/files/{fileId}/{version} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/ActiveConfig (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-ActiveConfig~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/allreferences?configId={configId}&folderId={folderId}&includeSubParents={includeSubParents} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-allreferences-configId%3D%7BconfigId%7D-folderId%3D%7BfolderId%7D-includeSubParents%3D%7BincludeSubParents%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/configurations (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-configurations~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/download (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-download~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/info (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-info~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/info/extended (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-info-extended~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/references?configId={configId}&folderId={folderId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-references-configId%3D%7BconfigId%7D-folderId%3D%7BfolderId%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/thumbnails (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-thumbnails~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/variables (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-variables~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/{version}/whereused?configId={configId}&folderId={folderId}&anyVersion={anyVersion} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-%7Bversion%7D-whereused-configId%3D%7BconfigId%7D-folderId%3D%7BfolderId%7D-anyVersion%3D%7BanyVersion%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/bominfo?folderId={folderId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-bominfo-folderId%3D%7BfolderId%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/info?version={version} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-info-version%3D%7Bversion%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/transitions?version={version} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-transitions-version%3D%7Bversion%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}/versions?folderId={folderId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-versions-folderId%3D%7BfolderId%7D~o-HttpGet.html)* [api/{vaultName}/files/{fileId}?destroy={destroy} (Delete)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-destroy%3D%7Bdestroy%7D~o-HttpDelete.html)* [api/{vaultName}/files/{fileId}?version={version} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BfileId%7D-version%3D%7Bversion%7D~o-HttpGet.html)* [api/{vaultName}/files/buildtree/checkout (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-buildtree-checkout~o-HttpPost.html)* [api/{vaultName}/files/buildtree/undo (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-buildtree-undo~o-HttpPost.html)* [api/{vaultName}/files/CheckOut (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-CheckOut~o-HttpPost.html)* [api/{vaultName}/files/info (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-info~o-HttpPost.html)* [api/{vaultName}/files/UndoCheckOut (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-UndoCheckOut~o-HttpPost.html)

###### [Folder](PDM%20Pro%20API_ws~g-c7793cfc-a764-4894-97ae-8cbe544c3bec.html)

* [api/{vaultName}/folders/{folderId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D~o-HttpGet.html)* [api/{vaultName}/folders/{folderId}/browse (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D-browse~o-HttpGet.html)* [api/{vaultName}/folders/{folderId}/info (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-info~o-HttpPost.html)* [api/{vaultName}/folders/{folderId}?destroy={destroy} (Delete)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D-destroy%3D%7Bdestroy%7D~o-HttpDelete.html)* [api/{vaultName}/folders/{parentFolderId} (Put)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-%7BfolderId%7D~o-HttpGet.html)* [api/{vaultName}/folders/info (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-folders-info~o-HttpPost.html)

###### [Group](PDM%20Pro%20API_ws~g-da825d69-2b4a-4cdc-ba87-51fea91e9c21.html)

* [api/{vaultName}/groups (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-groups~o-HttpGet.html)* [api/{vaultName}/groups/{groupId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-groups-%7BgroupId%7D~o-HttpGet.html)* [api/{vaultName}/groups/{groupId}/info (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-groups-%7BgroupId%7D-info~o-HttpGet.html)* [api/{vaultName}/groups/all (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-groups-all~o-HttpGet.html)

###### [Notification](PDM%20Pro%20API_ws~g-8ab41ef0-9f61-4e69-ac2a-5eb2be677c1b.html)

* [api/{vaultName}/notifications (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-notifications~o-HttpPost.html)* [api/{vaultName}/notifications/markRead (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-notifications-markRead~o-HttpPost.html)* [api/{vaultName}/notifications?all={all}&pageNo={pageNo}&pageSize={pageSize} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-notifications-all%3D%7Ball%7D-pageNo%3D%7BpageNo%7D-pageSize%3D%7BpageSize%7D~o-HttpGet.html)

###### [Progress](PDM%20Pro%20API_ws~g-da460c84-0fe1-4150-989d-fdd62d69ef3b.html)

* [api/{vaultName}/progress/{guid}/result (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-progress-%7Bguid%7D-result~o-HttpGet.html)* [api/{vaultName}/progress/{guid}/status (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-progress-%7Bguid%7D-status~o-HttpGet.html)

###### [Stage](PDM%20Pro%20API_ws~g-e97ee2e8-3e51-4fe9-991a-ddc5b293f468.html)

* [api/{vaultName}/changeset/create (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-changeset-create~o-HttpGet.html)* [api/{vaultName}/checkin/{changesetId}/{overrideVersion} (Put)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-%7BchangesetId%7D-%7BoverrideVersion%7D~o-HttpPut.html)* [api/{vaultName}/checkin/addfiles/{changesetId} (Put)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-addfiles-%7BchangesetId%7D~o-HttpPut.html)* [api/{vaultName}/checkin/buildtree/{changesetId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-checkin-buildtree-%7BchangesetId%7D~o-HttpGet.html)* [api/{vaultName}/files/{changesetId}/finishadd (Put)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BchangesetId%7D-finishadd~o-HttpPut.html)* [api/{vaultName}/files/{changesetId}/upload (Put)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-files-%7BchangesetId%7D-upload~o-HttpPut.html)

###### [State Transition](PDM%20Pro%20API_ws~g-d61f95b6-4b32-4c36-a0ec-956478ec12e0.html)

* [api/{vaultName}/state/{documentId}/{folderId}/{transitionId}/references (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BdocumentId%7D-%7BfolderId%7D-%7BtransitionId%7D-references~o-HttpGet.html)* [api/{vaultName}/state/{documentId}/transitions (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BdocumentId%7D-transitions~o-HttpGet.html)* [api/{vaultName}/state/{transitionId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D~o-HttpGet.html)* [api/{vaultName}/state/{transitionId}/changestate?revoke={revoke} (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-changestate-revoke%3D%7Brevoke%7D~o-HttpPost.html)* [api/{vaultName}/state/{transitionId}/DynamicNotificationUsers (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-DynamicNotificationUsers~o-HttpPost.html)* [api/{vaultName}/state/{transitionId}/HistoryComments (Post](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-%7BtransitionId%7D-HistoryComments~o-HttpPost.html))* [api/{vaultName}/state/transitions (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-state-transitions~o-HttpPost.html)

###### [User](PDM%20Pro%20API_ws~g-cdc45fab-a6bc-420b-bd83-e00f27db722f.html)

* [api/{vaultName}/users (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users~o-HttpGet.html)* [api/{vaultName}/users/{userId} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D~o-HttpGet.html)* [api/{vaultName}/users/{userId}/Extended (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Extended~o-HttpGet.html)* [api/{vaultName}/users/{userId}/Extended (Put)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Extended~o-HttpPut.html)* [api/{vaultName}/users/{userId}/info (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-info~o-HttpGet.html)* [api/{vaultName}/users/{userId}/Picture (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Picture~o-HttpGet.html)* [api/{vaultName}/users/{userId}/Picture (Put)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Picture~o-HttpPut.html)* [api/{vaultName}/users/{userId}/Picture (Delete)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-%7BuserId%7D-Picture~o-HttpDelete.html)* [api/{vaultName}/users/all (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-users-all~o-HttpGet.html)

###### [Vault](PDM%20Pro%20API_ws~g-c5af818a-41e9-4b86-9ff8-123e7de9800d.html)

* [api/{vaultName} (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D~o-HttpGet.html)* [api/{vaultName}/delete/computetree (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-delete-computetree~o-HttpPost.html)* [api/{vaultName}/info (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-info~o-HttpGet.html)* [api/{vaultName}/search (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-search~o-HttpGet.html)* [api/{vaultName}/search (Post)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-search~o-HttpPost.html)

###### [Version](PDM%20Pro%20API_ws~g-d109c663-82c9-4f09-ae1a-d25359a6e2fd.html)

* [api/version/webapi (Get)](PDM%20Pro%20API_ws~r-api-version-webapi~o-HttpGet.html)

###### [Workflow](PDM%20Pro%20API_ws~g-00a18afc-82ee-4f15-88c4-b4e2aaa3e88e.html)

* [api/{vaultName}/workflows (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-workflows~o-HttpGet.html)* [api/{vaultName}/workflows/icons (Get)](PDM%20Pro%20API_ws~r-api-%7BvaultName%7D-workflows-icons~o-HttpGet.html)