<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout~GetTargetPoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetTargetPoint Method (ICallout) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICallout Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout.html) : GetTargetPoint Method (ICallout) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RowID*
:   Row in callout

*XPos*
:   x coordinate of target point

*YPos*
:   y coordinate of target point

*ZPos*
:   z coordinate of target point

Gets the target point for the specified row in this callout.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetTargetPoint( _    ByVal RowID As System.Integer, _    ByRef XPos As System.Double, _    ByRef YPos As System.Double, _    ByRef ZPos As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICallout Dim RowID As System.Integer Dim XPos As System.Double Dim YPos As System.Double Dim ZPos As System.Double   instance.GetTargetPoint(RowID, XPos, YPos, ZPos) ``` | |

| C# |  |
| --- | --- |
| ``` void GetTargetPoint(     System.int RowID,    out System.double XPos,    out System.double YPos,    out System.double ZPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetTargetPoint(  &   System.int RowID, &   [Out] System.double XPos, &   [Out] System.double YPos, &   [Out] System.double ZPos ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RowID*
:   Row in callout

*XPos*
:   x coordinate of target point

*YPos*
:   y coordinate of target point

*ZPos*
:   z coordinate of target point

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Callout::GetTargetPoint.

# ![](dotnetimages/collapse.gif)See Also

####

[ICallout Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout.html)

[ICallout Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout_members.html)

[ICallout::SetTargetPoint Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout~SetTargetPoint.html)

[ICallout::UpdatePosition Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout~UpdatePosition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15