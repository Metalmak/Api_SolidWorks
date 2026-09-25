<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDistanceMateFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IDistanceMateFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a distance mate or a limit distance mate feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IDistanceMateFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDistanceMateFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IDistanceMateFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IDistanceMateFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DistanceMateFeatureData.

# ![](dotnetimages/collapse.gif)Example

[Create and Edit Limit Distance Mate (VBA)](Create_Limit_Distance_Mate_Example_VB.htm)

[Create and Edit Limit Distance Mate (C#)](Create_Limit_Distance_Mate_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A distance mate places selected items at a specified distance. A limit distance mate is an advanced mate that allows components to move within a range of distances. Use [IDistanceMateFeatureData::IsAdvancedMate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData~IsAdvancedMate.html) to determine whether this is a limit distance mate.

[IMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateFeatureData.html) is the parent of this mate interface.

To create either a distance mate or a limit distance mate:

1. Follow general instructions in the [IAssemblyDoc::CreateMate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateMate.html) Remarks.- Specify [IDistanceMateFeatureData::EntitiesToMate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData~EntitiesToMate.html) or use [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to pre-select the entities using Mark = 1.- Specify other properties of the DistanceMateFeatureData object.

To edit a distance mate:

1. Access its feature and call [IFeature::GetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html) to get the MateFeatureData object.- Cast the MateFeatureData object to a DistanceMateFeatureData object.- Modify the DistanceMateFeatureData object.- Call [IFeature::ModifyDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ModifyDefinition.html).

To delete a distance mate, use [IModelDocExtension::DeleteSelection2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteSelection2.html).

# ![](dotnetimages/collapse.gif)Access Diagram

[DistanceMateFeatureData](SWObjectModel.pdf#DistanceMateFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[IDistanceMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDistanceMateFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)