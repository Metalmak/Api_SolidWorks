<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdNode~GetProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetProperty Method (IEdmCmdNode) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCmdNode Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdNode.html) : GetProperty Method (IEdmCmdNode) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eProperty*
:   Type of property to retrieve as defined in [EdmCmdNodeProp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdNodeProp.html)

*oArg*
:   Null; reserved for future use

Gets the specified property for the file changing state.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetProperty( _    ByVal eProperty As EdmCmdNodeProp, _    Optional ByVal oArg As System.Object _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetProperty(     EdmCmdNodeProp eProperty,    System.object oArg ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetProperty(  &   EdmCmdNodeProp eProperty, &   System.Object^ oArg ) ``` | |

#### Parameters

*eProperty*
:   Type of property to retrieve as defined in [EdmCmdNodeProp](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdNodeProp.html)

*oArg*
:   Null; reserved for future use

#### Return Value

Property value

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCmdNode](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdNode.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCmdNode Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdNode.html)

[IEdmCmdNode Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdNode_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011