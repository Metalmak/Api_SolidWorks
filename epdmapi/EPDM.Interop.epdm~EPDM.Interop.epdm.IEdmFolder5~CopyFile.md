<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CopyFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CopyFile Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : CopyFile Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file to copy

*lSrcFolderID*
:   ID of folder from which to copy the file

*lParentWnd*
:   Parent window handle

*bsNewName*
:   Optional new name of the file; "" to use the original file name

*lFlags*
:   Combination of [EdmCopyFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyFlag.html) bits

Obsolete. Superseded by [IEdmFolder8::CopyFile2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8~CopyFile2.html)

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CopyFile( _    ByVal lFileID As System.Integer, _    ByVal lSrcFolderID As System.Integer, _    ByVal lParentWnd As System.Integer, _    Optional ByVal bsNewName As System.String, _    Optional ByVal lFlags As System.Integer _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int CopyFile(     System.int lFileID,    System.int lSrcFolderID,    System.int lParentWnd,    System.string bsNewName,    System.int lFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CopyFile(  &   System.int lFileID, &   System.int lSrcFolderID, &   System.int lParentWnd, &   System.String^ bsNewName, &   System.int lFlags ) ``` | |

#### Parameters

*lFileID*
:   ID of file to copy

*lSrcFolderID*
:   ID of folder from which to copy the file

*lParentWnd*
:   Parent window handle

*bsNewName*
:   Optional new name of the file; "" to use the original file name

*lFlags*
:   Combination of [EdmCopyFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCopyFlag.html) bits

#### Return Value

ID of the new file

# ![](dotnetimages/collapse.gif)Example

[Vault Utilities (C#)](Add_File_Example_CSharp.htm)

[Vault Utilities (VB.NET)](Add_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method uses the ID of a file to identify which file to copy. You can also call [IEdmFolder5::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFile.html), specifying the path of the file that you want to copy. IEdmFolder5::AddFile handles both source files that are inside and outside of the vault.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_NAME\_ALREADY\_EXISTS: There is already a file or folder with the same name in this folder.* E\_EDM\_FILE\_NOT\_FOUND: The source file was not found. (The ID is invalid.)* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to copy the specified file.* E\_EDM\_FILE\_SHARE\_ERROR: Cannot copy the file because it is exclusively opened in another application.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the installed [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreCopy hooks didn't permit the operation.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

[IEdmFolder5::AddFileShared Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFileShared.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2