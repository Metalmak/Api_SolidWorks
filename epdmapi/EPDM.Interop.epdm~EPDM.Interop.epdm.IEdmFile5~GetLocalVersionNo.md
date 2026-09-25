<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetLocalVersionNo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetLocalVersionNo Method (IEdmFile5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html) : GetLocalVersionNo Method (IEdmFile5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPathOrFolderID*
:   ID of a folder, full file path, or folder path of the local copy of this file (see **Remarks**)

Obsolete. Superseded by [IEdmFile12::GetLocalVersionNo2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile12~GetLocalVersionNo2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetLocalVersionNo( _    ByRef poPathOrFolderID As System.Object _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetLocalVersionNo(     ref System.object poPathOrFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetLocalVersionNo(  &   System.Object^% poPathOrFolderID ) ``` | |

#### Parameters

*poPathOrFolderID*
:   ID of a folder, full file path, or folder path of the local copy of this file (see **Remarks**)

#### Return Value

Version number; -1 if the local copy does not match any version in the archive

# ![](dotnetimages/collapse.gif)Example

[Get File Information (VB.NET)](Get_File_Info_Example_VBNET.htm)

[Get File Information (C#)](Get_File_Info_Example_CSharp.htm)

[Get Revision Names for Local Version of File (C#)](Get_Revision_Names_for_Local_Version_of_File_Example_CSharp.htm)

[Get Revision Names for Local Version of File (VB.NET)](Get_Revision_Names_for_Local_Version_of_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

If poPathOrFolderID is a folder path, it must be terminated by a backslash ('\').

See [Return Codes](ReturnCodes.htm) for the complete list of potential success and error codes. The following are just a few examples:

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5.html)

[IEdmFile5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2