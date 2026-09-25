<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~GetFileCopy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFileCopy Method (IEdmVersion5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5.html) : GetFileCopy Method (IEdmVersion5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*poPathOrFolderID*
:   ID or path of the folder where to copy the file; 0 to place a copy of the file in all of its shared folders (default) (see **Remarks**)

*lEdmGetFlags*
:   Optional combination of [EdmGetFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html) bits; default is EdmGetFlag.EdmGet\_MakeReadOnly

*bsNewName*
:   Optional new name of the copied file; "" to create a copy using the file's current name

Retrieves from the archive a copy of this version of a file and places it in the specified location.

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
:   ID or path of the folder where to copy the file; 0 to place a copy of the file in all of its shared folders (default) (see **Remarks**)

*lEdmGetFlags*
:   Optional combination of [EdmGetFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html) bits; default is EdmGetFlag.EdmGet\_MakeReadOnly

*bsNewName*
:   Optional new name of the copied file; "" to create a copy using the file's current name

# ![](dotnetimages/collapse.gif)Example

[Check Out and Copy File (VB.NET)](Check_Out_and_Copy_File_Example_VBNET.htm)

[Check Out and Copy File (C#)](Check_Out_and_Copy_File_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you specify a folder path in poPathOrFolderID, it must be terminated by a backslash ('\').

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_FILE\_NOT\_FOUND: The file was not found in the vault.* E\_EDM\_PERMISSION\_DENIED: The user is not permitted to see the specified version of the file.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5.html)

[IEdmVersion5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5_members.html)

[IEdmFile5::GetFileCopy Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFileCopy.html)

[IEdmRevision5::GetFileCopy Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5~GetFileCopy.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2