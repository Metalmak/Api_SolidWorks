<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~SetEdgeAngleFilter.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| SetEdgeAngleFilter Method (IPowerSelect) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html) : SetEdgeAngleFilter Method (IPowerSelect) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*lCmpOperator*
:   Comparison operator as defined in [gtpslEdgeAngleOperator\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtpslEdgeAngleOperator_e.html)

*dAngle*
:   Angle in radians

Sets the Edge angle filter for this PowerSelect session.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetEdgeAngleFilter( _    ByVal lCmpOperator As System.Integer, _    ByVal dAngle As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPowerSelect Dim lCmpOperator As System.Integer Dim dAngle As System.Double Dim value As System.Integer   value = instance.SetEdgeAngleFilter(lCmpOperator, dAngle) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetEdgeAngleFilter(     System.int lCmpOperator,    System.double dAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetEdgeAngleFilter(  &   System.int lCmpOperator, &   System.double dAngle ) ``` | |

#### Parameters

*lCmpOperator*
:   Comparison operator as defined in [gtpslEdgeAngleOperator\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtpslEdgeAngleOperator_e.html)

*dAngle*
:   Angle in radians

#### Return Value

Error as defined in [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IPowerSelect::SetEdgeAngleFilter.

# ![](dotnetimages/collapse.gif)See Also

####

[IPowerSelect Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html)

[IPowerSelect Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect_members.html)

[IPowerSelect::GetEdgeAngleFilter Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect~GetEdgeAngleFilter.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2005 FCS