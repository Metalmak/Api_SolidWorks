<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8~CopyFile2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CopyFile2 Method (IEdmFolder8) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8.html) : CopyFile2 Method (IEdmFolder8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of the file to copy

*lSrcFolderID*
:   ID of the folder from which to copy the file

*lParentWnd*
:   Parent window handle

*plErrorCode*
:   * 0 indicates that the file is copied* [EdmResultSuccessCodes\_e.](EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode.EdmResultSuccessCodes_e.html)S\_EDM\_FILES\_NOT\_UNIQUE\_GLOBALLY indicates that the file is copied if you are copying the file to a different folder in the vault; otherwise, the file is not copied

*bsNewName*
:   Optional new name of the file; "" to use the original file name

*lFlags*
:   Combination of [EdmAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html) bits

Copies a file from a different folder in the vault to this folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CopyFile2( _    ByVal lFileID As System.Integer, _    ByVal lSrcFolderID As System.Integer, _    ByVal lParentWnd As System.Integer, _    ByRef plErrorCode As System.Integer, _    Optional ByVal bsNewName As System.String, _    Optional ByVal lFlags As System.Integer _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int CopyFile2(     System.int lFileID,    System.int lSrcFolderID,    System.int lParentWnd,    out System.int plErrorCode,    System.string bsNewName,    System.int lFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CopyFile2(  &   System.int lFileID, &   System.int lSrcFolderID, &   System.int lParentWnd, &   [Out] System.int plErrorCode, &   System.String^ bsNewName, &   System.int lFlags ) ``` | |

#### Parameters

*lFileID*
:   ID of the file to copy

*lSrcFolderID*
:   ID of the folder from which to copy the file

*lParentWnd*
:   Parent window handle

*plErrorCode*
:   * 0 indicates that the file is copied* [EdmResultSuccessCodes\_e.](EPDM.Interop.EPDMResultCode~EPDM.Interop.EPDMResultCode.EdmResultSuccessCodes_e.html)S\_EDM\_FILES\_NOT\_UNIQUE\_GLOBALLY indicates that the file is copied if you are copying the file to a different folder in the vault; otherwise, the file is not copied

*bsNewName*
:   Optional new name of the file; "" to use the original file name

*lFlags*
:   Combination of [EdmAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html) bits

#### Return Value

ID of the new file

# ![](dotnetimages/collapse.gif)Example

[Copy File (C#)](Copy_File_Example_CSharp.htm)

[Copy File (VB.NET)](Copy_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method uses the ID of a file to copy a file inside the vault. Use [IEdmFolder8::AddFile2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8~AddFile2.html) to copy a file by its path. IEdmFolder8::AddFile2 can handle source files both inside and outside the vault.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_NAME\_ALREADY\_EXISTS: There is already a file or folder with the same name in this folder.* E\_EDM\_FILE\_NOT\_FOUND: The source file was not found. (The ID is invalid.)* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to copy the specified file.* E\_EDM\_FILE\_SHARE\_ERROR: Cannot copy the file because it is exclusively opened in another application.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the installed [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreCopy hooks didn't permit the operation.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8.html)

[IEdmFolder8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015