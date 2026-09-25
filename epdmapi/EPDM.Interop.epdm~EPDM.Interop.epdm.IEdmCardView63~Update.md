<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView63~Update.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Update Method (IEdmCardView63) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardView63 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView63.html) : Update Method (IEdmCardView63) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of update to perform as defined in [EdmCardViewUpdateType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewUpdateType.html)

*poArg*
:   Reserved for future use

Updates controls in this card view.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Update( _    ByVal eType As EdmCardViewUpdateType, _    Optional ByRef poArg As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Update(     EdmCardViewUpdateType eType,    ref System.object poArg ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Update(  &   EdmCardViewUpdateType eType, &   System.Object^% poArg ) ``` | |

#### Parameters

*eType*
:   Type of update to perform as defined in [EdmCardViewUpdateType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardViewUpdateType.html)

*poArg*
:   Reserved for future use

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardView63](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView63.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardView63 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView63.html)

[IEdmCardView63 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardView63_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4