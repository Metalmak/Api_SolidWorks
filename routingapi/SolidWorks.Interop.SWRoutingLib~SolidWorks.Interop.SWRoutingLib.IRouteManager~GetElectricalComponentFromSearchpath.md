<!-- source: routingapi/SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager~GetElectricalComponentFromSearchpath.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Routing API Help | Send comments on this topic. |
| GetElectricalComponentFromSearchpath Method (IRouteManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.SWRoutingLib Namespace](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib_namespace.html) > [IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html) : GetElectricalComponentFromSearchpath Method (IRouteManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*\_\_MIDL\_\_IRouteManager0001*
:   File name of the routing component for which to search

Gets the path and file name of the electrical component.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetElectricalComponentFromSearchpath( _    ByVal __MIDL__IRouteManager0001 As System.String _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRouteManager Dim __MIDL__IRouteManager0001 As System.String Dim value As System.String   value = instance.GetElectricalComponentFromSearchpath(__MIDL__IRouteManager0001) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetElectricalComponentFromSearchpath(     System.string __MIDL__IRouteManager0001 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetElectricalComponentFromSearchpath(  &   System.String^ __MIDL__IRouteManager0001 ) ``` | |

#### Parameters

*\_\_MIDL\_\_IRouteManager0001*
:   File name of the routing component for which to search

#### Return Value

Path and file name of the electrical component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RouteManager::GetElectricalComponentFromSearchpath.

# ![](dotnetimages/collapse.gif)Remarks

If the specified routing component is not found, then the return value is empty.

# ![](dotnetimages/collapse.gif)See Also

####

[IRouteManager Interface](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager.html)

[IRouteManager Members](SolidWorks.Interop.SWRoutingLib~SolidWorks.Interop.SWRoutingLib.IRouteManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Routing 2007 FCS