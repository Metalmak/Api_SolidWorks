<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint~GetID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetID Method (ISketchPoint) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html) : GetID Method (ISketchPoint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the sketch point ID for this sketch point.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetID() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPoint Dim value As System.Object   value = instance.GetID() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetID() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetID(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array with two longs or two integers (see Long vs. Integer) identifying this sketch point ID

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchPoint::GetID.

# ![](dotnetimages/collapse.gif)Example

[Get Sketch Points and Sketch Point IDs (VBA)](Get_Sketch_Points_and_Their_Persistent_IDs_Example_VB.htm)

[Get x,y,z Locations of Points in Sketch (VBA)](Get_x%2Cy%2Cz_Locations_of_Points_in_Sketch_Example_VB.htm)

[Get Persistent Identifiers and Types for Sketch Points (VB.NET)](Get_Persistent_Identifiers_and_Types_for_Sketch_Points_Example_VBNET.htm)

[Get Persistent Identifiers and Types for Sketch Points (C#)](Get_Persistent_Identifiers_and_Types_for_Sketch_Points_Example_CSharp.htm)

[Get Sketch Relations (VBA)](Get_Sketch_Relations_Example_VB.htm)

[Get Sketch Relations (VB.NET)](Get_Sketch_Relations_Example_VBNET.htm)

[Get Sketch Relations (C#)](Get_Sketch_Relations_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The ID of the sketch point:

* is an ordered pair (i1, i2). For sketch points, the combination of these two numbers is always unique within a specific sketch.* cannot be assigned by applications or users.* is not the same as a persistent reference ID.

Each point within a specific sketch has a unique ID. However, a point and other sketch objects can have the same ID. Likewise, in a second sketch, you may find a different sketch element with the same ID. Therefore, your application must keep track of:

* sketch element type (that is, point, line, arc, spline, and so on)

  * owning sketch name

    * sketch element ID to uniquely identify a sketched item

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPoint Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html)

[ISketchPoint Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint_members.html)

[ISketchPoint::IGetID Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint~IGetID.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207