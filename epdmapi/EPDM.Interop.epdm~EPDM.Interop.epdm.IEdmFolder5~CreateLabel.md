<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateLabel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateLabel Method (IEdmFolder5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html) : CreateLabel Method (IEdmFolder5) |

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

*bRecursively*
:   Optionally, true to set the label recursively on subfolders, false to not; default is true

Creates a label on this folder and its subfolders.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateLabel( _    ByVal bsName As System.String, _    ByVal bsDescription As System.String, _    Optional ByVal bRecursively As System.Boolean _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateLabel(     System.string bsName,    System.string bsDescription,    System.bool bRecursively ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateLabel(  &   System.String^ bsName, &   System.String^ bsDescription, &   System.bool bRecursively ) ``` | |

#### Parameters

*bsName*
:   Name of the label; maximum of 255 characters

*bsDescription*
:   Label description to show in the history dialog box; maximum of 2000 characters

*bRecursively*
:   Optionally, true to set the label recursively on subfolders, false to not; default is true

#### Return Value

ID of the new label

# ![](dotnetimages/collapse.gif)Example

[Create Labels on Folders (VB.NET)](Create_Label_Example_VBNET.htm)

[Create Labels on Folders (C#)](Create_Label_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments in invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFolder5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html)

[IEdmFolder5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5_members.html)

[IEdmLabel5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel5.html)

[IEdmFolder5::GetFirstLabelPosition Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~GetFirstLabelPosition.html)

[IEdmFile16::CreateLabel Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile16~CreateLabel.html)

[IEdmEnumeratorVersion5::CreateLabel Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5~CreateLabel.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2