<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector~Find.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| Find Method (IAdvancedRouteSelector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IAdvancedRouteSelector Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html) : Find Method (IAdvancedRouteSelector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*connectorName*
:   Component name; can be the name of a fitting, cable, or wire; can include wild-card character (\*)

*searchType*
:   Search type as defined by swRoutingSearchType\_e

*singleInstanceOnly*
:   True to find a single instance of connectorName, false to find all instances of connectorName

*append*
:   True appends the selection to the selection list, false replaces the selection list with this selection

Finds the number of specified components in the assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Find( _    ByVal connectorName As System.String, _    ByVal searchType As System.Integer, _    ByVal singleInstanceOnly As System.Boolean, _    ByVal append As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedRouteSelector Dim connectorName As System.String Dim searchType As System.Integer Dim singleInstanceOnly As System.Boolean Dim append As System.Boolean Dim value As System.Integer   value = instance.Find(connectorName, searchType, singleInstanceOnly, append) ``` | |

| C# |  |
| --- | --- |
| ``` System.int Find(     System.string connectorName,    System.int searchType,    System.bool singleInstanceOnly,    System.bool append ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Find(  &   System.String^ connectorName, &   System.int searchType, &   System.bool singleInstanceOnly, &   System.bool append ) ``` | |

#### Parameters

*connectorName*
:   Component name; can be the name of a fitting, cable, or wire; can include wild-card character (\*)

*searchType*
:   Search type as defined by swRoutingSearchType\_e

*singleInstanceOnly*
:   True to find a single instance of connectorName, false to find all instances of connectorName

*append*
:   True appends the selection to the selection list, false replaces the selection list with this selection

#### Return Value

Number of components found for connectorName

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedRouteSelector::Find.

# ![](dotnetimages/collapse.gif)Example

See the [IAdvancedRouteSelector](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedRouteSelector Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector.html)

[IAdvancedRouteSelector Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IAdvancedRouteSelector_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2009 FCS