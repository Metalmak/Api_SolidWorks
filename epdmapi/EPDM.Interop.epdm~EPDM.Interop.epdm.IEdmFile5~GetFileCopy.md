<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFileCopy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFileCopy Method (IEdmFile5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : GetFileCopy Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*poVersionNoOrRevisionName*
:   Version number or revision name of the file to get; 0 or "" to get the latest version

*poPathOrFolderID*
:   Optional folder ID or path where to deposit the file; default is to deposit the file in all of its parent folders (see **Remarks**)

*lEdmGetFlags*
:   Optional combination of [EdmGetFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html) bits; default is EdmGetFlag.EdmGet\_MakeReadOnly

*bsNewName*
:   Optional new name of the copy of this file; empty string to use the file's current name

Gets a copy of the file with the specified version from the archive and deposits it in the specified location.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetFileCopy( _    ByVal lParentWnd As System.Integer, _    Optional ByRef poVersionNoOrRevisionName As System.Object, _    Optional ByRef poPathOrFolderID As System.Object, _    Optional ByVal lEdmGetFlags As System.Integer, _    Optional ByVal bsNewName As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFileCopy(     System.int lParentWnd,    ref System.object poVersionNoOrRevisionName,    ref System.object poPathOrFolderID,    System.int lEdmGetFlags,    System.string bsNewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFileCopy(  &   System.int lParentWnd, &   System.Object^% poVersionNoOrRevisionName, &   System.Object^% poPathOrFolderID, &   System.int lEdmGetFlags, &   System.String^ bsNewName ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*poVersionNoOrRevisionName*
:   Version number or revision name of the file to get; 0 or "" to get the latest version

*poPathOrFolderID*
:   Optional folder ID or path where to deposit the file; default is to deposit the file in all of its parent folders (see **Remarks**)

*lEdmGetFlags*
:   Optional combination of [EdmGetFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html) bits; default is EdmGetFlag.EdmGet\_MakeReadOnly

*bsNewName*
:   Optional new name of the copy of this file; empty string to use the file's current name

# ![](dotnetimages/collapse.gif)Example

[Add Files to Vault (VB.NET)](Add_Files_to_Vault_Example_VBNET.htm)

[Add Files to Vault (C#)](Add_Files_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If poPathOrFolderID = 0, then the file is copied to all folders to which this file is shared. If poPathOrFolderID is a folder path, it must be terminated by a backslash ('\').

To retrieve several files, use [IEdmBatchGet](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchGet.html), which is more efficient than calling this method several times.

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_REVISION\_NUMBER: The revision was not found.* E\_EDM\_PERMISSION\_DENIED: The logged-in user lacks permission to see the specified version of the file.* E\_EDM\_FILE\_NOT\_FOUND: The file was not found in the vault.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

[IEdmFile5::LockFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~LockFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2