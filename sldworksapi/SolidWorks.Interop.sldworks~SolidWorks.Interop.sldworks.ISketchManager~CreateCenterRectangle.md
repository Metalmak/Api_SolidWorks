<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateCenterRectangle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateCenterRectangle Method (ISketchManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : CreateCenterRectangle Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X1*
:   X coordinate for point 1

*Y1*
:   Y coordinate for point 1

*Z1*
:   Z coordinate for point 1

*X2*
:   X coordinate for point 2

*Y2*
:   Y coordinate for point 2

*Z2*
:   Z coordinate for point 2

Creates a center rectangle.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateCenterRectangle( _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Z1 As System.Double, _    ByVal X2 As System.Double, _    ByVal Y2 As System.Double, _    ByVal Z2 As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim X1 As System.Double Dim Y1 As System.Double Dim Z1 As System.Double Dim X2 As System.Double Dim Y2 As System.Double Dim Z2 As System.Double Dim value As System.Object   value = instance.CreateCenterRectangle(X1, Y1, Z1, X2, Y2, Z2) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateCenterRectangle(     System.double X1,    System.double Y1,    System.double Z1,    System.double X2,    System.double Y2,    System.double Z2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateCenterRectangle(  &   System.double X1, &   System.double Y1, &   System.double Z1, &   System.double X2, &   System.double Y2, &   System.double Z2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X1*
:   X coordinate for point 1

*Y1*
:   Y coordinate for point 1

*Z1*
:   Z coordinate for point 1

*X2*
:   X coordinate for point 2

*Y2*
:   Y coordinate for point 2

*Z2*
:   Z coordinate for point 2

#### Return Value

Array of [sketch segments](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html) that represent the edges and diagonals created for this center rectangle

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::CreateCenterRectangle.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchManager::Create3PointCenterRectangle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~Create3PointCenterRectangle.html)

[ISketchManager::Create3PointCornerRectangle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~Create3PointCornerRectangle.html)