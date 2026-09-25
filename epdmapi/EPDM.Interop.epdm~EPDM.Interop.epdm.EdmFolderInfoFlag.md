<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfoFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmFolderInfoFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmFolderInfoFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Return codes in [EdmFolderInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo.html) which is returned from [IEdmBatchAddFolders::Create](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAddFolders~Create.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmFolderInfoFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmFolderInfoFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmFolderInfoFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Eff\_AlreadyExisted** | 1 = Folder already existed in the vault; [EdmFolderInfo structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderInfo.html) contains information about the existing folder |
| **Eff\_Nothing** | 0 = Folder was successfully added |
| **Eff\_PermissionDenied** | 2 = Folder could not be added due to lack of permissions |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)