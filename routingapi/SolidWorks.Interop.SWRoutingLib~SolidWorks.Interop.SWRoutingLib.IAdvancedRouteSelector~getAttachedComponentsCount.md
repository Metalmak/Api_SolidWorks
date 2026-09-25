<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector~getAttachedComponentsCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| getAttachedComponentsCount Method (IAdvancedRouteSelector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAdvancedRouteSelector Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html) : getAttachedComponentsCount Method (IAdvancedRouteSelector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*selIndex*
:   Index of the component whose number of attached components you want

Gets the number of attached components for the specified component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function getAttachedComponentsCount( _    ByVal selIndex As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedRouteSelector Dim selIndex As System.Integer Dim value As System.Integer   value = instance.getAttachedComponentsCount(selIndex) ``` | |

| C# |  |
| --- | --- |
| ``` System.int getAttachedComponentsCount(     System.int selIndex ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int getAttachedComponentsCount(  &   System.int selIndex ) ``` | |

#### Parameters

*selIndex*
:   Index of the component whose number of attached components you want

#### Return Value

Number of attached components for the component corresponding to selIndex

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedRouteSelector::getAttachedComponentsCount.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedRouteSelector](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedRouteSelector Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html)

[IAdvancedRouteSelector Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2009 FCS