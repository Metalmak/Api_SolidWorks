<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UndoLockFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| UndoLockFile Method (IEdmFile5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : UndoLockFile Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*bGetLatestVersion*
:   Optional; true to replace the local copy of the file with the latest from the archive, false to not; default is true

Removes the check-out of a file without saving changes to the archive.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub UndoLockFile( _    ByVal lParentWnd As System.Integer, _    Optional ByVal bGetLatestVersion As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void UndoLockFile(     System.int lParentWnd,    System.bool bGetLatestVersion ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void UndoLockFile(  &   System.int lParentWnd, &   System.bool bGetLatestVersion ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*bGetLatestVersion*
:   Optional; true to replace the local copy of the file with the latest from the archive, false to not; default is true

# ![](dotnetimages/collapse.gif)Example

[Access File Card Variables (VB.NET)](Access_File_Card_Variables_Example_VBNET.htm)

[Access File Card Variables (C#)](Access_File_Card_Variables_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, the file must be checked out by the logged-in user.

[IEdmBatchUnlock](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUnlock.html) is more efficient than this interface for undoing the check-outs of multiple files.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_LOCKED\_BY\_YOU: The file is not checked out or is checked out by another user.* E\_EDM\_LOCKED\_ON\_OTHER\_COMPUTER: The file is not checked out on the client machine where you ran this method.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the loaded [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreUndoLock hooks did not permit the operation.* E\_EDM\_PERMISSION\_DENIED: Undoing the check-out of this file is not permitted. You cannot undo the check-out of a file before it has been checked in at least once.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

[IEdmFile5::UnlockFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~UnlockFile.html)

[IEdmfile5::LockFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2