<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateParabola.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateParabola Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : CreateParabola Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*XFocus*
:   X coordinate for the focus

*YFocus*
:   Y coordinate for the focus

*ZFocus*
:   Z coordinate for the focus

*XApex*
:   X coordinate for the apex

*YApex*
:   Y coordinate for the apex

*ZApex*
:   Z coordinate for the apex

*X1*
:   X coordinate for the start point

*Y1*
:   Y coordinate for the start point

*Z1*
:   Z coordinate for the start point

*X2*
:   X coordinate for the end point

*Y2*
:   Y coordinate for the end point

*Z2*
:   Z coordinate for the end point

Creates a parabola in the active sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateParabola( _    ByVal XFocus As System.Double, _    ByVal YFocus As System.Double, _    ByVal ZFocus As System.Double, _    ByVal XApex As System.Double, _    ByVal YApex As System.Double, _    ByVal ZApex As System.Double, _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Z1 As System.Double, _    ByVal X2 As System.Double, _    ByVal Y2 As System.Double, _    ByVal Z2 As System.Double _ ) As SketchSegment ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim XFocus As System.Double Dim YFocus As System.Double Dim ZFocus As System.Double Dim XApex As System.Double Dim YApex As System.Double Dim ZApex As System.Double Dim X1 As System.Double Dim Y1 As System.Double Dim Z1 As System.Double Dim X2 As System.Double Dim Y2 As System.Double Dim Z2 As System.Double Dim value As SketchSegment   value = instance.CreateParabola(XFocus, YFocus, ZFocus, XApex, YApex, ZApex, X1, Y1, Z1, X2, Y2, Z2) ``` | |

| C# |  |
| --- | --- |
| ``` SketchSegment CreateParabola(     System.double XFocus,    System.double YFocus,    System.double ZFocus,    System.double XApex,    System.double YApex,    System.double ZApex,    System.double X1,    System.double Y1,    System.double Z1,    System.double X2,    System.double Y2,    System.double Z2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchSegment^ CreateParabola(  &   System.double XFocus, &   System.double YFocus, &   System.double ZFocus, &   System.double XApex, &   System.double YApex, &   System.double ZApex, &   System.double X1, &   System.double Y1, &   System.double Z1, &   System.double X2, &   System.double Y2, &   System.double Z2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*XFocus*
:   X coordinate for the focus

*YFocus*
:   Y coordinate for the focus

*ZFocus*
:   Z coordinate for the focus

*XApex*
:   X coordinate for the apex

*YApex*
:   Y coordinate for the apex

*ZApex*
:   Z coordinate for the apex

*X1*
:   X coordinate for the start point

*Y1*
:   Y coordinate for the start point

*Z1*
:   Z coordinate for the start point

*X2*
:   X coordinate for the end point

*Y2*
:   Y coordinate for the end point

*Z2*
:   Z coordinate for the end point

#### Return Value

[Sketch segment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html) for the parabola

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::CreateParabola.

# ![](dotnetimages/collapse.gif)Example

[Create Parabola (VBA)](Create_Parabola_Example_VB.htm)

[Create Parabola (VB.NET)](Create_Parabola_Example_VBNET.htm)

[Create Parabola (C#)](Create_Parabola_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchManager::CreateConic Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateConic.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0