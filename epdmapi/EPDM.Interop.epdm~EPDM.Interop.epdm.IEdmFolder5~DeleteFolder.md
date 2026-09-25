<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| DeleteFolder Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : DeleteFolder Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*lSubfolderID*
:   ID of folder to delete

*bRemoveLocalCopy*
:   Optionally true to remove the folder from the local disk, false to not; default is true

Deletes the specified subfolder from this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub DeleteFolder( _    ByVal lParentWnd As System.Integer, _    ByVal lSubfolderID As System.Integer, _    Optional ByVal bRemoveLocalCopy As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void DeleteFolder(     System.int lParentWnd,    System.int lSubfolderID,    System.bool bRemoveLocalCopy ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DeleteFolder(  &   System.int lParentWnd, &   System.int lSubfolderID, &   System.bool bRemoveLocalCopy ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*lSubfolderID*
:   ID of folder to delete

*bRemoveLocalCopy*
:   Optionally true to remove the folder from the local disk, false to not; default is true

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method deletes only folders that are empty.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FOLDER\_NOT\_FOUND: The specified ID is not a subfolder of this folder.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the installed [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreDeleteFolder hooks did not permit the operation.* E\_EDM\_FOLDER\_NOT\_EMPTY: The folder cannot be deleted, because it has files or subfolders in it.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to delete the specified folder.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

[IEdmFolder5::DeleteFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFile.html)

[IEdmFolder11::RecoverDeletedItems Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11~RecoverDeletedItems.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2