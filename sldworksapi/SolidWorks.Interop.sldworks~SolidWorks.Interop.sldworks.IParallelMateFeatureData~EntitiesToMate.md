<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParallelMateFeatureData~EntitiesToMate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EntitiesToMate Property (IParallelMateFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IParallelMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParallelMateFeatureData.html) : EntitiesToMate Property (IParallelMateFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the entities to mate in this parallel mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EntitiesToMate As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IParallelMateFeatureData Dim value As System.Object   instance.EntitiesToMate = value   value = instance.EntitiesToMate ``` | |

| C# |  |
| --- | --- |
| ``` System.object EntitiesToMate {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ EntitiesToMate {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Entities to mate (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ParallelMateFeatureData::EntitiesToMate.

# ![](dotnetimages/collapse.gif)Example

See the [IParallelMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParallelMateFeatureData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

You can create parallel mates with the following mate entity combinations:

| Mate entity/Mate entity | [IRefAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)  (cone, cylinder) | IFace2  (extrusion face,  draft is not allowed) | [IEdge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html),  IRefAxis,  [ICenterLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterLine.html),  [ISketchLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html)  (line) | [IRefPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html) | [ISurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html),  IFace2  (non-analytic  surface) |
| --- | --- | --- | --- | --- | --- |
| **IRefAxis (cone, cylinder)** | ● | ● | ● |  | ● |
| **IFace2 (extrusion face,**  **draft is not allowed)** | ● | ● | ● |  |  |
| **IEdge, IRefAxis, ICenterLine, ISketchLine (line)** | ● | ● | ● | ● | ● |
| **IRefPlane** |  |  | ● | ● |  |
| **ISurface, IFace2**  **(non-analytic surface)** | ● |  | ● |  |  |

Instead of specifying this property, you can use [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to pre-select the entities to mate using Mark = 1. You can pre-select mate entities during mate creation, but not during mate editing.

# ![](dotnetimages/collapse.gif)See Also

####

[IParallelMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParallelMateFeatureData.html)

[IParallelMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IParallelMateFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0