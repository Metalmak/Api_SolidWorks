<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2~SweepPlanarLoop.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SweepPlanarLoop Method (ILoop2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ILoop2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2.html) : SweepPlanarLoop Method (ILoop2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X component of the sweep vector

*Y*
:   Y component of the sweep vector

*Z*
:   Z component of the sweep vector

*DraftAngle*
:   Draft angle for the faces on the side of this swept body

Creates a temporary body by sweeping a planar loop along a vector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SweepPlanarLoop( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double, _    ByVal DraftAngle As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILoop2 Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim DraftAngle As System.Double Dim value As System.Object   value = instance.SweepPlanarLoop(X, Y, Z, DraftAngle) ``` | |

| C# |  |
| --- | --- |
| ``` System.object SweepPlanarLoop(     System.double X,    System.double Y,    System.double Z,    System.double DraftAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ SweepPlanarLoop(  &   System.double X, &   System.double Y, &   System.double Z, &   System.double DraftAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   X component of the sweep vector

*Y*
:   Y component of the sweep vector

*Z*
:   Z component of the sweep vector

*DraftAngle*
:   Draft angle for the faces on the side of this swept body

#### Return Value

Array containing new swept [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html) (element 1) and two stop [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) (elements 2 and 3)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Loop2::SweepPlanarLoop.

# ![](dotnetimages/collapse.gif)Example

[Sweep Planar Loop Along Vector (VBA)](Sweep_Planar_Loop_Along_Vector_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method requires simplification of the imported body.

# ![](dotnetimages/collapse.gif)See Also

####

[ILoop2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2.html)

[ILoop2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2_members.html)

[ILoop2::ISweepPlanarLoop Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILoop2~ISweepPlanarLoop.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0