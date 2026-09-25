<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoincidentMateFeatureData~EntitiesToMate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EntitiesToMate Property (ICoincidentMateFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICoincidentMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoincidentMateFeatureData.html) : EntitiesToMate Property (ICoincidentMateFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the entities to mate in this coincident mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EntitiesToMate As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICoincidentMateFeatureData Dim value As System.Object   instance.EntitiesToMate = value   value = instance.EntitiesToMate ``` | |

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

See CoincidentMateFeatureData::EntitiesToMate.

# ![](dotnetimages/collapse.gif)Example

See the [ICoincidentMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoincidentMateFeatureData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

Instead of specifying this property, you can use [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to pre-select the entities to mate using Mark = 1. You can pre-select mate entities during mate creation, but not during mate editing.

Populate the array of this property by using either IModelDocExtension::SelectByID2 or [IModelDocExtension::SelectByRay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByRay.html) and [ISelectionMgr::GetSelectedObject6](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html).

Create coincident mates with the following mate entity combinations:

| Mate entity/Mate entity | [IEdge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html)  (arc, circular edge) | [ISurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurface.html),  [IFace2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)  (cone) | [IFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)  (coordinate system) | [ICurve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)  (arc, spline, helix) | ISurface,  IFace2  (cylinder) | IFace2  (extrusion face, draft is not allowed) | IEdge,  [IRefAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html),  [ICenterLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICenterLine.html),  [ISketchLine](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html)  (line) | [IEntity](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity.html)  (coordinate system origin) | [IRefPlane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html) | [IRefPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPoint.html),  [IVertex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex.html),  [ISketchPoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html) | ISurface,  IFace2  (sphere) | ISurface |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| **IEdge (arc, circular edge)** | ● | ● |  |  | ● |  |  |  | ● | ● |  |  |
| **ISurface, IFace2 (cone)** | ● | ● Both cones must be of the same half angle |  |  |  |  |  |  |  | ● |  |  |
| **IFeature (coordinate system)** |  |  | ● |  |  |  |  | ● |  |  |  |  |
| **ICurve (arc, spline, helix)** |  |  |  |  |  |  |  |  |  | ● |  |  |
| **ISurface, IFace2 (cylinder)** | ● |  |  |  |  |  | ● |  |  |  |  |  |
| **IFace2 (extrusion face, draft is not allowed)** |  |  |  |  |  |  |  |  |  | ● |  |  |
| **IEdge, IRefAxis, ICenterLine, ISketchLine (line)** |  |  |  |  | ● |  | ● |  | ● | ● |  |  |
| **IEntity (coordinate system origin)** |  |  | ● |  |  |  |  | ● |  |  |  |  |
| **IRefPlane** | ● |  |  |  |  |  | ● |  | ● | ● |  |  |
| **IRefPoint, IVertex, ISketchPoint** | ● | ● |  | ● | ● | ● | ● |  | ● | ● | ● | ● |
| **ISurface, IFace2 (sphere)** |  |  |  |  |  |  |  |  |  | ● |  |  |
| **ISurface** |  |  |  |  |  |  |  |  |  | ● |  |  |

After specifying the entities to mate, specify their [ICoincidentMateFeatureData::PickPoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoincidentMateFeatureData~PickPoints.html) to fully define the position of the mate.

# ![](dotnetimages/collapse.gif)See Also

####

[ICoincidentMateFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoincidentMateFeatureData.html)

[ICoincidentMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoincidentMateFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0