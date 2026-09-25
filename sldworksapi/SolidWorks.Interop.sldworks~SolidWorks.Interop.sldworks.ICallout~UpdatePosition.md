<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout~UpdatePosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UpdatePosition Method (ICallout) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICallout Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout.html) : UpdatePosition Method (ICallout) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XPos*
:   x coordinate for callout

*YPos*
:   y coordinate for callout

*ZPos*
:   z coordinate for callout

Obsolete. Superseded by [Callout::Position](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICallout~Position.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub UpdatePosition( _    ByVal XPos As System.Double, _    ByVal YPos As System.Double, _    ByVal ZPos As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICallout Dim XPos As System.Double Dim YPos As System.Double Dim ZPos As System.Double   instance.UpdatePosition(XPos, YPos, ZPos) ``` | |

| C# |  |
| --- | --- |
| ``` void UpdatePosition(     System.double XPos,    System.double YPos,    System.double ZPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void UpdatePosition(  &   System.double XPos, &   System.double YPos, &   System.double ZPos ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XPos*
:   x coordinate for callout

*YPos*
:   y coordinate for callout

*ZPos*
:   z coordinate for callout

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Callout::UpdatePosition.

# ![](dotnetimages/collapse.gif)See Also

####

[ICallout Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout.html)

[ICallout Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICallout_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15