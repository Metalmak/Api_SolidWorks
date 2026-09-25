<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile9~GetLocalFileSize2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetLocalFileSize2 Method (IEdmFile9) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile9.html) : GetLocalFileSize2 Method (IEdmFile9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPathOrFolderID*
:   ID of the folder, a full file path, or a folder path (see **Remarks**)

Gets the size of a local copy of this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetLocalFileSize2( _    ByRef poPathOrFolderID As System.Object _ ) As System.Long ``` | |

| C# |  |
| --- | --- |
| ``` System.long GetLocalFileSize2(     ref System.object poPathOrFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int64 GetLocalFileSize2(  &   System.Object^% poPathOrFolderID ) ``` | |

#### Parameters

*poPathOrFolderID*
:   ID of the folder, a full file path, or a folder path (see **Remarks**)

#### Return Value

Size in bytes; -1 if the local file is missing

# ![](dotnetimages/collapse.gif)Example

[Get File Information (VB.NET)](Get_File_Info_Example_VBNET.htm)

[Get File Information (C#)](Get_File_Info_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If poPathOrFolderID is a folder path, it must be terminated by a backslash ('\').

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The local copy of the file is missing.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile9.html)

[IEdmFile9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile9_members.html)

[IEdmFile5::GetLocalFileDate Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalFileDate.html)

[IEdmFile5::GetLocalRevisionName Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalRevisionName.html)

[IEdmFile5::GetLocalVersionNo Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalVersionNo.html)

[IEdmVersion5::FileSize Property ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~FileSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015