<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5~GetFileCopy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFileCopy Method (IEdmRevision5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevision5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5.html) : GetFileCopy Method (IEdmRevision5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*poPathOrFolderID*
:   Path or ID of the folder where to place the file; default copies the file to all of the folders to which it is shared (see **Remarks**)

*lEdmGetFlags*
:   Optional combination of [EdmGetFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html) bits; default is EdmGetFlag.EdmGet\_MakeReadOnly

*bsNewName*
:   Optional new name of the file copy; "" to use the file's current name

Gets a copy of this revision of the file from the archive and places it in the specified folder on the client machine.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetFileCopy( _    ByVal lParentWnd As System.Integer, _    Optional ByRef poPathOrFolderID As System.Object, _    Optional ByVal lEdmGetFlags As System.Integer, _    Optional ByVal bsNewName As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFileCopy(     System.int lParentWnd,    ref System.object poPathOrFolderID,    System.int lEdmGetFlags,    System.string bsNewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFileCopy(  &   System.int lParentWnd, &   System.Object^% poPathOrFolderID, &   System.int lEdmGetFlags, &   System.String^ bsNewName ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*poPathOrFolderID*
:   Path or ID of the folder where to place the file; default copies the file to all of the folders to which it is shared (see **Remarks**)

*lEdmGetFlags*
:   Optional combination of [EdmGetFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html) bits; default is EdmGetFlag.EdmGet\_MakeReadOnly

*bsNewName*
:   Optional new name of the file copy; "" to use the file's current name

# ![](dotnetimages/collapse.gif)Remarks

If you specify a path for poPathOrFolderID, you can either give a file path or a folder path. Folder paths must be terminated by a backslash ('\').

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_FOUND: The file was not found in the vault.* E\_EDM\_PERMISSION\_DENIED: The user is not permitted to see the specified version of the file.* E\_EDM\_INVALID\_REVISION\_NUMBER: The revision was not found.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevision5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5.html)

[IEdmRevision5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2