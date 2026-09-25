<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetArcEndCondition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetArcEndCondition Method (IDimension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html) : SetArcEndCondition Method (IDimension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Index*
:   Index of the endpoint on which to set the end condition; 1 is the first endpoint, 2 is the second endpoint

*Condition*
:   End condition as defined in swArcEndCondition\_e

Sets the end conditions for linear dimensions that end on an arc.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetArcEndCondition( _    ByVal Index As System.Integer, _    ByVal Condition As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimension Dim Index As System.Integer Dim Condition As System.Integer Dim value As System.Integer   value = instance.SetArcEndCondition(Index, Condition) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetArcEndCondition(     System.int Index,    System.int Condition ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetArcEndCondition(  &   System.int Index, &   System.int Condition ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Index*
:   Index of the endpoint on which to set the end condition; 1 is the first endpoint, 2 is the second endpoint

*Condition*
:   End condition as defined in swArcEndCondition\_e

#### Return Value

Indicates the success or failure of this method:

|  |  |
| --- | --- |
| 0 | Command was successful; the arc end condition was set |
| -1 | Command failed for an unknown reason; the arc end condition was not set |
| -2 | Index parameter is invalid |
| -3 | Condition parameter is invalid |
| -4 | Endpoint 1 is not related to an arc |
| -5 | Endpoint 2 is not related to an arc |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Dimension::SetArcEndCondition.

# ![](dotnetimages/collapse.gif)Remarks

Linear dimensions measure the distance from one point to another. If one or both of those points is on an arc, the point can be changed to the center point of the arc, the nearest point on the arc, or the furthest point on the arc. The arc end condition describes which point to use.

Use [IDimension::GetArcEndCondition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~GetArcEndCondition.html) to get the arc end conditions.

To see the effects of changing the arc endpoint conditions, use [IModelDoc2::GraphicsRedraw2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GraphicsRedraw2.html) to redraw the graphics window.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html)

[IDimension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension_members.html)

[IDimension::GetArcEndCondition Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetArcEndCondition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207