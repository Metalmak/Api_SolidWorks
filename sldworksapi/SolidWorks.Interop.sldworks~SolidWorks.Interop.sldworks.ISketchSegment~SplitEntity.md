<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~SplitEntity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SplitEntity Method (ISketchSegment) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html) : SplitEntity Method (ISketchSegment) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   x coordinate where to split the selected entity

*Y*
:   y coordinate where to split the selected entity

*Z*
:   z coordinate where to split the selected entity

*ClosedX*
:   x coordinate where to close the split entity

*ClosedY*
:   y coordinate where to close the split entity

*ClosedZ*
:   z coordinate where to close the split entity

Splits the selected sketch entity at the specified point.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SplitEntity( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByVal ClosedX As System.Double, _    ByVal ClosedY As System.Double, _    ByVal ClosedZ As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchSegment Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim ClosedX As System.Double Dim ClosedY As System.Double Dim ClosedZ As System.Double   instance.SplitEntity(X, Y, Z, ClosedX, ClosedY, ClosedZ) ``` | |

| C# |  |
| --- | --- |
| ``` void SplitEntity(     System.double X,    System.double Y,    System.double Z,    System.double ClosedX,    System.double ClosedY,    System.double ClosedZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SplitEntity(  &   System.double X, &   System.double Y, &   System.double Z, &   System.double ClosedX, &   System.double ClosedY, &   System.double ClosedZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   x coordinate where to split the selected entity

*Y*
:   y coordinate where to split the selected entity

*Z*
:   z coordinate where to split the selected entity

*ClosedX*
:   x coordinate where to close the split entity

*ClosedY*
:   y coordinate where to close the split entity

*ClosedZ*
:   z coordinate where to close the split entity

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchSegment::SplitEntity.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

[ISketchSegment Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 17.0