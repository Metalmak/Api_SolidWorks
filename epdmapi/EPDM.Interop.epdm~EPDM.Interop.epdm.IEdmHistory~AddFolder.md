<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~AddFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFolder Method (IEdmHistory) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmHistory Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html) : AddFolder Method (IEdmHistory) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFolderID*
:   ID of folder to add

*lEdmFolderHistoryFlags*
:   Combination of [EdmFolderHistoryFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderHistoryFlag.html) bits (see **Remarks**)

Adds a folder to the history listing.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddFolder( _    ByVal lFolderID As System.Integer, _    ByVal lEdmFolderHistoryFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddFolder(     System.int lFolderID,    System.int lEdmFolderHistoryFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddFolder(  &   System.int lFolderID, &   System.int lEdmFolderHistoryFlags ) ``` | |

#### Parameters

*lFolderID*
:   ID of folder to add

*lEdmFolderHistoryFlags*
:   Combination of [EdmFolderHistoryFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmFolderHistoryFlag.html) bits (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

lEdmFolderHistoryFlags indicates whether subfolders are added recursively and whether files in the specified folder are added.

After all the files and folders have been added, call [IEdmHistory::GetHistory](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory~GetHistory.html) to obtain the actual history listing.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistory Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory.html)

[IEdmHistory Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistory_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4