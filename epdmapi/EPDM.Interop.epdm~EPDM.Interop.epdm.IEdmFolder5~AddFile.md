<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddFile Method (IEdmFolder5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : AddFile Method (IEdmFolder5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle

*bsSrcPath*
:   Path of file to copy; "" to create an empty file with name specified by bsNewFileName (see **Remarks**)

*bsNewFileName*
:   Optional new file name; "" to use the file name specified in bsSrcPath (see **Remarks**)

*lEdmAddFlags*
:   Combination of [EdmAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html) bits

Obsolete. Superseded by [IEdmFolder8::AddFile2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder8~AddFile2.html)

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function AddFile( _    ByVal lParentWnd As System.Integer, _    ByVal bsSrcPath As System.String, _    Optional ByVal bsNewFileName As System.String, _    Optional ByVal lEdmAddFlags As System.Integer _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddFile(     System.int lParentWnd,    System.string bsSrcPath,    System.string bsNewFileName,    System.int lEdmAddFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddFile(  &   System.int lParentWnd, &   System.String^ bsSrcPath, &   System.String^ bsNewFileName, &   System.int lEdmAddFlags ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle

*bsSrcPath*
:   Path of file to copy; "" to create an empty file with name specified by bsNewFileName (see **Remarks**)

*bsNewFileName*
:   Optional new file name; "" to use the file name specified in bsSrcPath (see **Remarks**)

*lEdmAddFlags*
:   Combination of [EdmAddFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html) bits

#### Return Value

ID of the new file

# ![](dotnetimages/collapse.gif)Remarks

Use this method to:

* copy a file from another folder that is either inside or outside of the vault.* create a new empty file.

Use:

* [IEdmFolder5::CopyFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CopyFile.html) to copy files within the vault.* [IEdmFolder5::AddFileShared](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFileShared.html) to share files between folders.

To add multiple files to this folder, use [IEdmFolder6::AddFiles](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder6~AddFiles.html) to add them all at once, which is more efficient than adding them one at a time using this method.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to add files to this folder.* E\_EDM\_NAME\_ALREADY\_EXISTS: There is already a file with the specified name in this folder.* E\_EDM\_INVALID\_NAME: The suggested file name is invalid.* E\_EDM\_FILE\_SHARE\_ERROR: The source or destination file is opened exclusively by another program.* E\_EDM\_FILE\_NOT\_FOUND: The source file could not be found.* E\_EDM\_OPERATION\_REFUSED\_BY\_PLUGIN: One of the installed [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreAdd hooks did not permit the operation.

To create a virtual document in a folder, pass an empty string as the source file. For example:

:   :   ```
        eFolder.AddFile(Me.Handle.ToInt32, '', path, 0)
        ```

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

[IEdmFolder5::AddFileShared Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFileShared.html)

[IEdmFolder5::CopyFile Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CopyFile.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2