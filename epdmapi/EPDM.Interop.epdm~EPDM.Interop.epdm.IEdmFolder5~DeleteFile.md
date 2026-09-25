<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| DeleteFile Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : DeleteFile Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*lFileID*
:   ID of file to delete

*bRemoveLocalCopy*
:   Optionally, true to erase the local copy of the file, false to not; default is true

Deletes a file having the specified ID from this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub DeleteFile( _    ByVal lParentWnd As System.Integer, _    ByVal lFileID As System.Integer, _    Optional ByVal bRemoveLocalCopy As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void DeleteFile(     System.int lParentWnd,    System.int lFileID,    System.bool bRemoveLocalCopy ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DeleteFile(  &   System.int lParentWnd, &   System.int lFileID, &   System.bool bRemoveLocalCopy ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*lFileID*
:   ID of file to delete

*bRemoveLocalCopy*
:   Optionally, true to erase the local copy of the file, false to not; default is true

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (VB.NET)](Vault_Utilities_Example_VBNET.htm)

[Vault Utilities (C#)](Vault_Utilities_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the specified file is shared to other folders, it is deleted only from this folder.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_FOUND: The file ID is invalid.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: The operation is not permitted by one of the installed [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreDelete hooks.* E\_EDM\_LOCKED\_BY\_ANOTHER\_USER: The file cannot be deleted since it is checked out by another user.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to delete the file.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

[IEdmFolder5::DeleteFolder Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~DeleteFolder.html)

[IEdmFolder11::RecoverDeletedItems Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder11~RecoverDeletedItems.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2