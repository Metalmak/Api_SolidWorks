<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentTrimExtendFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IWeldmentTrimExtendFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentTrimExtendFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IWeldmentTrimExtendFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to the data that defines a weldment trim extend feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IWeldmentTrimExtendFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IWeldmentTrimExtendFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IWeldmentTrimExtendFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IWeldmentTrimExtendFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See WeldmentTrimExtendFeatureData.

# ![](dotnetimages/collapse.gif)Example

[Get Weldment Trim Extend Corner Type (VBA)](Get_Weldment_Trim_Extend_Corner_Type_Example_VB.htm)

[Get Weldment Trim Extend Corner Type (VB.NET)](Get_Weldment_Trim_Extend_Corner_Type_Example_VBNET.htm)

[Get Weldment Trim Extend Corner Type (C#)](Get_Weldment_Trim_Extend_Corner_Type_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Only bodies created by weldment features can be trimmed and extended. Only End Trim corner types can have multiple target and boundary bodies to trim. All
other corner types can have only one target and boundary body to trim. For all other corner types, first valid body specified is used if more than one body is
specified.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html) and [IFeature::IGetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IGetDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[WeldmentTrimExtendFeatureData](SWObjectModel.pdf#WeldmentTrimExtendFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[IWeldmentTrimExtendFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWeldmentTrimExtendFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::InsertWeldmentTrimFeature2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertWeldmentTrimFeature2.html)

[IFeatureManager::InsertWeldmentTrimFeature Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertWeldmentTrimFeature.html)