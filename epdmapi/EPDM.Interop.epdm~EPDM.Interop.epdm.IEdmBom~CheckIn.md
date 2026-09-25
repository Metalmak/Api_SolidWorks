<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom~CheckIn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CheckIn Method (IEdmBom) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html) : CheckIn Method (IEdmBom) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsComment*
:   Comment to add to the history of this BOM

Checks in this BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub CheckIn( _    ByVal bsComment As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void CheckIn(     System.string bsComment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void CheckIn(  &   System.String^ bsComment ) ``` | |

#### Parameters

*bsComment*
:   Comment to add to the history of this BOM

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html)

[IEdmBom Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009