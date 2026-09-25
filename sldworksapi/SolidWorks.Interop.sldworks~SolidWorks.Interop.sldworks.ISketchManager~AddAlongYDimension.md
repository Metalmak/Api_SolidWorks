<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongYDimension.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddAlongYDimension Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : AddAlongYDimension Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X coordinate of dimension text placement

*Y*
:   Y coordinate of dimension text placement

*Z*
:   Z coordinate of dimension text placement

Projects and displays along the y axis a dimension between selected points in a 3D sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddAlongYDimension( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) As DisplayDimension ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As DisplayDimension   value = instance.AddAlongYDimension(X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` DisplayDimension AddAlongYDimension(     System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` DisplayDimension^ AddAlongYDimension(  &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   X coordinate of dimension text placement

*Y*
:   Y coordinate of dimension text placement

*Z*
:   Z coordinate of dimension text placement

#### Return Value

[IDisplayDimension](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDisplayDimension.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::AddAlongYDimension.

# ![](dotnetimages/collapse.gif)Example

[Add Along Y Dimension to 3D Sketch (VBA)](Add_Along_Y_Dimension_To_3D_Sketch_Example_VB.htm)

[Add Along Y Dimension to 3D Sketch (VB.NET)](Add_Along_Y_Dimension_To_3D_Sketch_Example_VBNET.htm)

[Add Along Y Dimension to 3D Sketch (C#)](Add_Along_Y_Dimension_To_3D_Sketch_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method works only for 3D sketches in edit mode, and the display dimension is visible only when the sketch is in edit mode.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchManager::FullyDefineSketch Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~FullyDefineSketch.html)

[ISketchManager::AddAlongXDimension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongXDimension.html)

[ISketchManager::AddAlongZDimension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongZDimension.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0