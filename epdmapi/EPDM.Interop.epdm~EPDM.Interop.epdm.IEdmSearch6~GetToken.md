<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6~GetToken.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetToken Method (IEdmSearch6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6.html) : GetToken Method (IEdmSearch6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eTok*
:   Type of token for which to get a value as defined in [EdmSearchToken](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSearchToken.html)

Gets the value of a search token.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetToken( _    ByVal eTok As EdmSearchToken _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetToken(     EdmSearchToken eTok ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetToken(  &   EdmSearchToken eTok ) ``` | |

#### Parameters

*eTok*
:   Type of token for which to get a value as defined in [EdmSearchToken](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSearchToken.html)

#### Return Value

Value of token

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6.html)

[IEdmSearch6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6_members.html)

[IEdmSearch6::SetToken Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch6~SetToken.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007