<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SplitClosedSegment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SplitClosedSegment Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SplitClosedSegment Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X0*
:   X value of first point

*Y0*
:   Y value of first point

*Z0*
:   Z value of first point

*X1*
:   X value of second point

*Y1*
:   Y value of second point

*Z1*
:   Z value of second point

Obsolete. Superseded by [ISketchManager::SplitClosedSegment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchManager~SplitClosedSegment.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SplitClosedSegment( _    ByVal X0 As System.Double, _    ByVal Y0 As System.Double, _    ByVal Z0 As System.Double, _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Z1 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim X0 As System.Double Dim Y0 As System.Double Dim Z0 As System.Double Dim X1 As System.Double Dim Y1 As System.Double Dim Z1 As System.Double   instance.SplitClosedSegment(X0, Y0, Z0, X1, Y1, Z1) ``` | |

| C# |  |
| --- | --- |
| ``` void SplitClosedSegment(     System.double X0,    System.double Y0,    System.double Z0,    System.double X1,    System.double Y1,    System.double Z1 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SplitClosedSegment(  &   System.double X0, &   System.double Y0, &   System.double Z0, &   System.double X1, &   System.double Y1, &   System.double Z1 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X0*
:   X value of first point

*Y0*
:   Y value of first point

*Z0*
:   Z value of first point

*X1*
:   X value of second point

*Y1*
:   Y value of second point

*Z1*
:   Z value of second point

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SplitClosedSegment.

# ![](dotnetimages/collapse.gif)Remarks

The selected sketch segment must be a closed entity (for example, the start and end points must be the same). To split a closed sketch segment (for example, a complete circle) into two pieces, you must specify two points (x1, y1, z1) and (x2, y2, z2).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::SplitOpenSegment Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SplitOpenSegment.html)

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0