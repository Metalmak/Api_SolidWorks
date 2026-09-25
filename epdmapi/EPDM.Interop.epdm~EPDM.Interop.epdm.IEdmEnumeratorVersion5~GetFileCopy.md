<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5~GetFileCopy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFileCopy Method (IEdmEnumeratorVersion5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5.html) : GetFileCopy Method (IEdmEnumeratorVersion5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle; 0 if none

*poVersionNoOrRevisionName*
:   Version number or revision string; 0 or "" to get the latest version

*poPathOrFolderID*
:   Optional ID or path of the folder where to deposit the file; default is to deposit in all of its parent folders (see **Remarks**)

*lEdmGetFlags*
:   Optional combination of [EdmGetFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html) bits; default is EdmGet\_MakeReadOnly

*bsNewName*
:   Optional new name for the retrieved file; "" indicates to use the file's current name

Retrieves a copy of a file with the specified version from the archive and deposits it in the specified folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetFileCopy( _    ByVal lParentWnd As System.Integer, _    ByRef poVersionNoOrRevisionName As System.Object, _    Optional ByRef poPathOrFolderID As System.Object, _    Optional ByVal lEdmGetFlags As System.Integer, _    Optional ByVal bsNewName As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetFileCopy(     System.int lParentWnd,    ref System.object poVersionNoOrRevisionName,    ref System.object poPathOrFolderID,    System.int lEdmGetFlags,    System.string bsNewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetFileCopy(  &   System.int lParentWnd, &   System.Object^% poVersionNoOrRevisionName, &   System.Object^% poPathOrFolderID, &   System.int lEdmGetFlags, &   System.String^ bsNewName ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle; 0 if none

*poVersionNoOrRevisionName*
:   Version number or revision string; 0 or "" to get the latest version

*poPathOrFolderID*
:   Optional ID or path of the folder where to deposit the file; default is to deposit in all of its parent folders (see **Remarks**)

*lEdmGetFlags*
:   Optional combination of [EdmGetFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html) bits; default is EdmGet\_MakeReadOnly

*bsNewName*
:   Optional new name for the retrieved file; "" indicates to use the file's current name

# ![](dotnetimages/collapse.gif)Example

See the example for [IEdmFile5::GetFileCopy](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFileCopy.html).

# ![](dotnetimages/collapse.gif)Remarks

If you specify a folder ID of 0 in poPathOrFolderID, SOLIDWORKS PDM Professional deposits the file in all of the folders it is shared to. If you specify a path in poPathOrFolderID, it can either be a file path or a folder path. Folder paths must be terminated by a backslash ('\').

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_FOUND: The file is not found in the vault.* E\_EDM\_PERMISSION\_DENIED: The user is not permitted to see the specified version of the file.* E\_EDM\_INVALID\_REVISION\_NUMBER: The revision is not found.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5.html)

[IEdmEnumeratorVersion5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2