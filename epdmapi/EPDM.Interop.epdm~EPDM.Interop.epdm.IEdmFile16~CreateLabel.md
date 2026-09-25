<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile16~CreateLabel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateLabel Method (IEdmFile16) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile16 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile16.html) : CreateLabel Method (IEdmFile16) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsName*
:   Name of the label; maximum of 255 characters

*bsDescription*
:   Label description to show in the history dialog box; maximum of 2000 characters

Creates a label with the specified name and description for this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateLabel( _    ByVal bsName As System.String, _    ByVal bsDescription As System.String _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateLabel(     System.string bsName,    System.string bsDescription ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateLabel(  &   System.String^ bsName, &   System.String^ bsDescription ) ``` | |

#### Parameters

*bsName*
:   Name of the label; maximum of 255 characters

*bsDescription*
:   Label description to show in the history dialog box; maximum of 2000 characters

#### Return Value

ID of the file label

# ![](dotnetimages/collapse.gif)Example

[Get File Information (VB.NET)](Get_File_Info_Example_VBNET.htm)

[Get File Information (C#)](Get_File_Info_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html) to get the [IEdmLabel5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5.html) object for this label.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments in invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile16 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile16.html)

[IEdmFile16 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile16_members.html)

[IEdmFolder5::CreateLabel Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateLabel.html)

[IEdmEnumeratorVersion5::CreateLabel Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5~CreateLabel.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2019 SP04