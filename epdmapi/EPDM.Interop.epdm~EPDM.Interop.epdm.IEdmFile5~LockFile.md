<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LockFile Method (IEdmFile5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : LockFile Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentFolderID*
:   ID of parent folder to which to check out the file

*lParentWnd*
:   Parent window handle

*lEdmLockFlags*
:   Optional combination of [EdmLockFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLockFlag.html) bits; default is EdmLockFlag.EdmLock\_Simple

Checks out this file from the vault to which the user is currently logged in.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub LockFile( _    ByVal lParentFolderID As System.Integer, _    ByVal lParentWnd As System.Integer, _    Optional ByVal lEdmLockFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void LockFile(     System.int lParentFolderID,    System.int lParentWnd,    System.int lEdmLockFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LockFile(  &   System.int lParentFolderID, &   System.int lParentWnd, &   System.int lEdmLockFlags ) ``` | |

#### Parameters

*lParentFolderID*
:   ID of parent folder to which to check out the file

*lParentWnd*
:   Parent window handle

*lEdmLockFlags*
:   Optional combination of [EdmLockFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmLockFlag.html) bits; default is EdmLockFlag.EdmLock\_Simple

# ![](dotnetimages/collapse.gif)Example

[Add Custom File Reference (VB.NET)](Add_Custom_File_Reference_Example_VBNET.htm)

[Add Custom File Reference (C#)](Add_Custom_File_Reference_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

When checking out several files, it is more efficient to use [IEdmBatchGet](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html) than to repeatedly call this method to check out every file.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_IS\_LOCKED: The file is already checked out.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to check out this file.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the installed [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreLock hooks did not permit the operation.* E\_EDM\_FILE\_NOT\_FOUND: The file was not found in the vault.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

[IEdmFile5::UnlockFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UnlockFile.html)

[IEdmFile5::UndoLockFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UndoLockFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2