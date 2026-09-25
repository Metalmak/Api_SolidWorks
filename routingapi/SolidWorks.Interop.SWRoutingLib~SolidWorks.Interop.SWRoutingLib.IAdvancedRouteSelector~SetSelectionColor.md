<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector~SetSelectionColor.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| SetSelectionColor Method (IAdvancedRouteSelector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAdvancedRouteSelector Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html) : SetSelectionColor Method (IAdvancedRouteSelector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*special*
:   True uses a specific color for selections, false does not

*colorIndex*
:   :   Integer value for RGB value

Sets the color of the selected components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetSelectionColor( _    ByVal special As System.Boolean, _    ByVal colorIndex As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedRouteSelector Dim special As System.Boolean Dim colorIndex As System.Integer   instance.SetSelectionColor(special, colorIndex) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSelectionColor(     System.bool special,    System.int colorIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSelectionColor(  &   System.bool special, &   System.int colorIndex ) ``` | |

#### Parameters

*special*
:   True uses a specific color for selections, false does not

*colorIndex*
:   :   Integer value for RGB value

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedRouteSelector::SetSelectionColor.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedRouteSelector](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedRouteSelector Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html)

[IAdvancedRouteSelector Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2009 FCS