<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~PerimeterCircle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PerimeterCircle Method (ISketchManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : PerimeterCircle Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X1*
:   coordinate for first point

*Y1*
:   y coordinate for first point

*X2*
:   x coordinate for second point

*Y2*
:   y coordinate for second point

*X3*
:   x coordinate for third point

*Y3*
:   y coordinate for third point

Draws a 3-point perimeter arc.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function PerimeterCircle( _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal X2 As System.Double, _    ByVal Y2 As System.Double, _    ByVal X3 As System.Double, _    ByVal Y3 As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim X1 As System.Double Dim Y1 As System.Double Dim X2 As System.Double Dim Y2 As System.Double Dim X3 As System.Double Dim Y3 As System.Double Dim value As System.Object   value = instance.PerimeterCircle(X1, Y1, X2, Y2, X3, Y3) ``` | |

| C# |  |
| --- | --- |
| ``` System.object PerimeterCircle(     System.double X1,    System.double Y1,    System.double X2,    System.double Y2,    System.double X3,    System.double Y3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ PerimeterCircle(  &   System.double X1, &   System.double Y1, &   System.double X2, &   System.double Y2, &   System.double X3, &   System.double Y3 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X1*
:   coordinate for first point

*Y1*
:   y coordinate for first point

*X2*
:   x coordinate for second point

*Y2*
:   y coordinate for second point

*X3*
:   x coordinate for third point

*Y3*
:   y coordinate for third point

#### Return Value

[3-point perimeter arc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchArc.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::PerimeterCircle.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0