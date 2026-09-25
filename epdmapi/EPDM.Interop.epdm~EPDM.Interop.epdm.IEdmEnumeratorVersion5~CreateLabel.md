<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5~CreateLabel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateLabel Method (IEdmEnumeratorVersion5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5.html) : CreateLabel Method (IEdmEnumeratorVersion5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsName*
:   Name of label; maximum 255 characters

*bsComment*
:   Label comment; maximum 2000 characters

Sets a label on the latest version of this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateLabel( _    ByVal bsName As System.String, _    ByVal bsComment As System.String _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int CreateLabel(     System.string bsName,    System.string bsComment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int CreateLabel(  &   System.String^ bsName, &   System.String^ bsComment ) ``` | |

#### Parameters

*bsName*
:   Name of label; maximum 255 characters

*bsComment*
:   Label comment; maximum 2000 characters

#### Return Value

ID of the label

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5.html)

[IEdmEnumeratorVersion5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5_members.html)

[IEdmFile16::CreateLabel Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile16~CreateLabel.html)

[IEdmFolder5::CreateLabel Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~CreateLabel.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2