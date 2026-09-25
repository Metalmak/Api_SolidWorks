<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData~EntitiesToMate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EntitiesToMate Property (IDistanceMateFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDistanceMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData.html) : EntitiesToMate Property (IDistanceMateFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the entities to mate in this distance mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EntitiesToMate As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDistanceMateFeatureData Dim value As System.Object   instance.EntitiesToMate = value   value = instance.EntitiesToMate ``` | |

| C# |  |
| --- | --- |
| ``` System.object EntitiesToMate {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ EntitiesToMate {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of entities to mate (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DistanceMateFeatureData::EntitiesToMate.

# ![](dotnetimages/collapse.gif)Example

See the [IDistanceMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

You can create distance mates with the following mate entity combinations:

| Mate entity/Mate entity | [IRefAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html),  [IFace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)  (cone) | [ICurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)  (arc, spline, helix) | IRefAxis,  IFace2  (cylinder) | [IEdge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html),  IRefAxis,  [ICenterLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterLine.html),  [ISketchLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html)  (line) | [IRefPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html),  IFace2 | [IRefPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPoint.html),  [IVertex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex.html),  [ISketchPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html) | [ISurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html),  IFace2  (sphere) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **IRefAxis, IFace2 (cone)** | ● Both cones must be of the same half angle |  |  |  |  |  |  |
| **ICurve (arc, spline, helix)** |  |  |  |  |  | ● |  |
| **IRefAxis, IFace2 (cylinder)** |  |  | ● | ● | ● | ● |  |
| **IEdge, IRefAxis, ICenterLine, ISketchLine (line)** |  |  | ● | ● | ● | ● | ● |
| **IRefPlane, IFace2** |  |  | ● | ● | ● | ● | ● |
| **IRefPoint, IVertex, ISketchPoint** |  | ● | ● | ● | ● | ● | ● |
| **ISurface, IFace2 (sphere)** |  |  |  | ● | ● | ● | ● |

# ![](dotnetimages/collapse.gif)See Also

####

[IDistanceMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData.html)

[IDistanceMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0