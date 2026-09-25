<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUtility.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmUtility Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmUtility Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Constants that are passed to the [IEdmVault7::CreateUtility](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault7~CreateUtility.html) to create utility interfaces of various kinds.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmUtility     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmUtility : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmUtility : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmUtil\_AddCustomRefs** | 8 = [IEdmAddCustomRefs](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddCustomRefs.html) |
| **EdmUtil\_BatchAdd** | 16 = [IEdmBatchAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) |
| **EdmUtil\_BatchAddFolders** | 14 = [IEdmBatchAddFolders](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders.html) |
| **EdmUtil\_BatchChangeState** | 22 = [IEdmBatchChangeState](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState.html) |
| **EdmUtil\_BatchDelete** | 20 = [IEdmBatchDelete](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchDelete.html) |
| **EdmUtil\_BatchGet** | 12 = [IEdmBatchGet](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) |
| **EdmUtil\_BatchItemGeneration** | 23 = [IEdmBatchItemGeneration](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration.html) |
| **EdmUtil\_BatchItemReferenceUpdate** | 25 = [IEdmBatchItemReferenceUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemReferenceUpdate.html) |
| **EdmUtil\_BatchList** | 13 = [IEdmBatchListing](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchListing.html) |
| **EdmUtil\_BatchRefVars** | 26 = [IEdmBatchRefVars](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchRefVars.html) |
| **EdmUtil\_BatchUnlock** | 6 = [IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) |
| **EdmUtil\_BatchUpdate** | 2 = [IEdmBatchUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html) |
| **EdmUtil\_BomMgr** | 24 = [IEdmBomMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomMgr.html) |
| **EdmUtil\_CategoryMgr** | 5 = [IEdmCategoryMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6.html) |
| **EdmUtil\_ClearLocalCache** | 19 = [IEdmClearLocalCache](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmClearLocalCache.html) |
| **EdmUtil\_FindUser** | 29 = [IEdmFindUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) |
| **EdmUtil\_History** | 17 = [IEdmHistory](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html) |
| **EdmUtil\_HistoryUpdate** | 21 = [IEdmHistoryUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate.html) |
| **EdmUtil\_RawReferenceMgr** | 15 = [IEdmRawReferenceMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRawReferenceMgr.html) |
| **EdmUtil\_RevisionMgr** | 18 = [IEdmRevisionMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr.html) |
| **EdmUtil\_Search** | 1 = [IEdmSearch5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html) (creates regular search objects only; to create an advanced search object, use [IEdmVault21::CreateSearch2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault21~CreateSearch2.html)) |
| **EdmUtil\_SerNoGen** | 11 = [IEdmSerNoGen6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen6.html) |
| **EdmUtil\_TaskMgr** | 30 = [IEdmTaskMgr](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskMgr.html) |
| **EdmUtil\_TemplateMgr** | 10 = [IEdmTemplateMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5.html) |
| **EdmUtil\_UpdateReferences** | 27 = [IEdmUpdateReferences](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUpdateReferences.html) |
| **EdmUtil\_UserMgr** | 3 = [IEdmUserMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html) |
| **EdmUtil\_VariableMgr** | 9 = [IEdmVariableMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5.html) |
| **EdmUtil\_WorkflowMgr** | 4 = [IEdmWorkflowMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmWorkflow6.html) |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)