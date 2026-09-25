<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint~Y.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Y Property (ISketchPoint) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html) : Y Property (ISketchPoint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets  the y coordinate of the sketch point.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Y As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPoint Dim value As System.Double   instance.Y = value   value = instance.Y ``` | |

| C# |  |
| --- | --- |
| ``` System.double Y {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double Y {    System.double get();    void set ( &   System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

y coordinate of the point location

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchPoint::Y.

# ![](dotnetimages/collapse.gif)Example

[Get All Elements of Sketch (VBA)](Get_All_Elements_of_Sketch_Example_VB.htm)

[Get Names of Sketch Segments (VBA)](Get_Names_of_Sketch_Segments_Example_VB.htm)

[Get Sketch Points (VBA)](Get_Sketch_Points_Example_VB.htm)

[Get x,y,z Locations of Points in Sketch (VBA)](Get_x%2Cy%2Cz_Locations_of_Points_in_Sketch_Example_VB.htm)

[Get Spline's Parameters (C#)](Get_Spline%27s_Parameters_Example_CSharp.htm)

[Get Spline's Parameters (VB.NET)](Get_Spline%27s_Parameters_Example_VBNET.htm)

[Get Spline's Parameters (VBA)](Get_Spline%27s_Parameters_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html)

[ISketchPoint Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint_members.html)

[ISketchPoint::X Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint~X.html)

[ISketchPoint::Z Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint~Z.html)

[ISketchPoint::SetCoords Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint~SetCoords.html)

[ISketchPoint::GetCoords Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint~GetCoords.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207