<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalFileSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetLocalFileSize Method (IEdmFile5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : GetLocalFileSize Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPathOrFolderID*
:   ID of the folder, a full file path, or a folder path (see **Remarks**)

Obsolete. Superseded by [IEdmFile9::GetLocalFileSize2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile9~GetLocalFileSize2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetLocalFileSize( _    ByRef poPathOrFolderID As System.Object _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetLocalFileSize(     ref System.object poPathOrFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetLocalFileSize(  &   System.Object^% poPathOrFolderID ) ``` | |

#### Parameters

*poPathOrFolderID*
:   ID of the folder, a full file path, or a folder path (see **Remarks**)

#### Return Value

Size in bytes; -1 if the local file is missing

# ![](dotnetimages/collapse.gif)Remarks

If poPathOrFolderID is a folder path, it must be terminated by a backslash ('\').

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* S\_FALSE: The local copy of the file is missing.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

[IEdmFile5::GetLocalFileDate Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalFileDate.html)

[IEdmFile5::GetLocalRevisionName Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalRevisionName.html)

[IEdmFile5::GetLocalVersionNo Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalVersionNo.html)

[IEdmVersion5::FileSize Property ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~FileSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2