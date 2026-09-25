<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChainPatternFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IChainPatternFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChainPatternFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IChainPatternFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a chain component pattern feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IChainPatternFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IChainPatternFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IChainPatternFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IChainPatternFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ChainPatternFeatureData.

# ![](dotnetimages/collapse.gif)Example

[Create and Modify Distance Chain Pattern Feature (C#)](Create_and_Modify_Distance_Chain_Pattern_Feature_Example_CSharp.htm)

[Create and Modify Distance Chain Pattern Feature (VB.NET)](Create_and_Modify_Distance_Chain_Pattern_Feature_Example_VBNET.htm)

[Create and Modify Distance Chain Pattern Feature (VBA)](Create_and_Modify_Distance_Chain_Pattern_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This interface supports the following chain component patterns:

* distance* distance linkage* connected linkage

Read Pattern Features and their Feature Data Objects.

Before calling IFeatureManager::CreateDefinition, you can pre-select the entities needed to populate the chain component pattern.

| Entity to select | Corresponding Chain Pattern PropertyManager control | Selection mark | Number of selections |
| --- | --- | --- | --- |
| * 2D or 3D [sketch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) containing an open or closed loop,* [Sketch line](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html), or* Model [edge](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) | **Path** | 2 | 1 for all types of chain patterns |
| Assembly [component](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html) | **Chain Group 1 Component to Pattern** | 1 | 1 for all types of chain patterns |
| * Cylindrical [face](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html),* Circular or linear edge,* [Sketch point](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPoint.html),* [Vertex](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex.html), or* [Reference axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html) | **Chain Group 1 Path Link 1** | 256 | 1 for all types of chain patterns |
| * Cylindrical face,* Circular or linear edge,* Sketch point,* Vertex, or* Reference axis | **Chain Group 1 Path Link 2** | 512 | * 1 for distance linkage or connected linkage* None for distance |
| Component [plane](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefPlane.html) or planar face | **Chain Group 1 Path Alignment Plane** | 16384 | 1 for all types of chain patterns |
| Assembly component | **Chain Group 2 Component to Pattern** | 2048 | * 1 for connected linkage* None for distance or linkage distance |
| * Cylindrical face,* Circular or linear edge,* Sketch point,* Vertex, or* Reference axis | **Chain Group 2 Path Link 1** | 4096 | * 1 for connected linkage* None for distance or linkage distance |
| * Cylindrical face,* Circular or linear edge,* Sketch point,* Vertex, or* Reference axis | **Chain Group 2 Path Link 2** | 8192 | * 1 for connected linkage* None for distance or linkage distance |
| Component plane or planar face | **Group 2 Path Alignment Plane** | 32768 | * 1 for connected linkage* None for distance or linkage distance |
| Assembly plane | **Face normal alignment** | 1024 | * 1 if the chain path is a sketch line* None for all other types of paths |

Or, after calling IFeatureManger::CreateDefinition, you can explicitly set the corresponding properties on the feature data object.

Either way, you must call [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) after initializing this feature data object in order to successfully create the chain component pattern feature.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html)

[IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[ChainPatternFeatureData](SWObjectModel.pdf#ChainPatternFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[IChainPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChainPatternFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)