<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateTangentArc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateTangentArc Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : CreateTangentArc Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X1*
:   X coordinate of start point in meters

*Y1*
:   Y coordinate of start point in meters

*Z1*
:   Z coordinate of start point in meters

*X2*
:   X coordinate of end point in meters

*Y2*
:   Y coordinate of end point in meters

*Z2*
:   Z coordinate of end point in meters

*ArcType*
:   Type of tangent arc as defined in swTangentArcTypes\_e

Creates a tangent arc.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateTangentArc( _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Z1 As System.Double, _    ByVal X2 As System.Double, _    ByVal Y2 As System.Double, _    ByVal Z2 As System.Double, _    ByVal ArcType As System.Integer _ ) As SketchSegment ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim X1 As System.Double Dim Y1 As System.Double Dim Z1 As System.Double Dim X2 As System.Double Dim Y2 As System.Double Dim Z2 As System.Double Dim ArcType As System.Integer Dim value As SketchSegment   value = instance.CreateTangentArc(X1, Y1, Z1, X2, Y2, Z2, ArcType) ``` | |

| C# |  |
| --- | --- |
| ``` SketchSegment CreateTangentArc(     System.double X1,    System.double Y1,    System.double Z1,    System.double X2,    System.double Y2,    System.double Z2,    System.int ArcType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchSegment^ CreateTangentArc(  &   System.double X1, &   System.double Y1, &   System.double Z1, &   System.double X2, &   System.double Y2, &   System.double Z2, &   System.int ArcType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X1*
:   X coordinate of start point in meters

*Y1*
:   Y coordinate of start point in meters

*Z1*
:   Z coordinate of start point in meters

*X2*
:   X coordinate of end point in meters

*Y2*
:   Y coordinate of end point in meters

*Z2*
:   Z coordinate of end point in meters

*ArcType*
:   Type of tangent arc as defined in swTangentArcTypes\_e

#### Return Value

[Sketch segment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html) of the tangent arc

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::CreateTangentArc.

# ![](dotnetimages/collapse.gif)Example

[Create Tangent Arc (VBA)](Create_Tangent_Arc_Example_VB.htm)

[Create Tangent Arc (VB.NET)](Create_Tangent_Arc_Example_VBNET.htm)

[Create Tangent Arc (C#)](Create_Tangent_Arc_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0