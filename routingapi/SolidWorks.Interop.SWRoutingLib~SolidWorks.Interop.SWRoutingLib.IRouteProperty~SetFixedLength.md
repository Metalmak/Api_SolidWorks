<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteProperty~SetFixedLength.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| SetFixedLength Method (IRouteProperty) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteProperty Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteProperty.html) : SetFixedLength Method (IRouteProperty) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NewLength*
:   Fixed length

Changes the length of a fixed-length route segment.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFixedLength( _    ByVal NewLength As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteProperty Dim NewLength As System.Double Dim value As System.Integer   value = instance.SetFixedLength(NewLength) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetFixedLength(     System.double NewLength ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetFixedLength(  &   System.double NewLength ) ``` | |

#### Parameters

*NewLength*
:   Fixed length

#### Return Value

Fixed length error code as defined in swSetRouteFixedLengthError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteProperty::SetFixedLength.

# ![](dotnetimages/collapse.gif)Example

See the [IRouteProperty](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteProperty.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method changes lengths only for route segments that have been constrained to have a fixed length in the SOLIDWORKS user interface. To constrain a route segment to a fixed length, right-click on the route segment and select **Fixed Length**.

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteProperty Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteProperty.html)

[IRouteProperty Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteProperty_members.html)

[IRouteProperty::GetFixedLength Method](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteProperty~GetFixedLength.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2009 SP4