<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6~GetDefaultValueComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetDefaultValueComponent Method (IEdmCardViewCallback6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardViewCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html) : GetDefaultValueComponent Method (IEdmCardViewCallback6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eValue*
:   Type of component for which to get a value as defined in [EdmDefValComp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDefValComp.html)

Called by the serial number generator to get the default value for the specified serial number component.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetDefaultValueComponent( _    ByVal eValue As EdmDefValComp _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetDefaultValueComponent(     EdmDefValComp eValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetDefaultValueComponent(  &   EdmDefValComp eValue ) ``` | |

#### Parameters

*eValue*
:   Type of component for which to get a value as defined in [EdmDefValComp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmDefValComp.html)

#### Return Value

Default value

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardViewCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

The user can generate a new serial number value in a card by right-clicking in the edit box linked to the serial number and selecting New Serial Number from the context menu. The serial number generator calls this method if it needs additional information in order to create the serial number. Implement this method to override the default behavior.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardViewCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6.html)

[IEdmCardViewCallback6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardViewCallback6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0