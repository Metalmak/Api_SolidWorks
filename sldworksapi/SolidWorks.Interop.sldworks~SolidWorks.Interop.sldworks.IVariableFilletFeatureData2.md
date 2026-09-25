<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IVariableFilletFeatureData2 Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IVariableFilletFeatureData2 Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a variable radius fillet feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IVariableFilletFeatureData2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IVariableFilletFeatureData2 ``` | |

| C# |  |
| --- | --- |
| ``` public interface IVariableFilletFeatureData2 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IVariableFilletFeatureData2 ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See VariableFilletFeatureData2.

# ![](dotnetimages/collapse.gif)Example

[Create Variable Radius Asymmetric Elliptical Fillet (VBA)](Create_Asymmetric_Elliptic_Fillets_Example_VB.htm)

[Create Variable Radius Asymmetric Elliptical Fillet (VB.NET)](Create_Asymmetric_Elliptic_Fillets_Example_VBNET.htm)

[Create Variable Radius Asymmetric Elliptical Fillet (C#)](Create_Asymmetric_Elliptic_Fillets_Example_CSharp.htm)

[Create Curvature Continuous Variable Fillet Feature (C#)](Create_Curvature_Continuous_Variable_Fillet_Feature_Example_CSharp.htm)

[Create Curvature Continuous Variable Fillet Feature (VB.NET)](Create_Curvature_Continuous_Variable_Fillet_Feature_Example_VBNET.htm)

[Create Curvature Continuous Variable Fillet Feature (VBA)](Create_Curvature_Continuous_Variable_Fillet_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

To create a variable fillet feature, follow the instructions in the Remarks section of [IFeatureManager::FeatureFillet3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureFillet3.html).

To edit a variable fillet feature:

1. Call [IFeature::GetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html).- Call [IVariableFilletFeatureData2::AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~AccessSelections.html).- Modify properties on this interface as needed and call [IFeature::ModifyDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ModifyDefinition.html).- If nothing is modified, call [IVariableFilletFeatureData2::ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2~ReleaseSelectionAccess.html).

For more information, read the **Variable Size Fillets** topic in the SOLIDWORKS user-interface help.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[VariableFilletFeatureData2](SWObjectModel.pdf#VariableFilletFeatureData2)

# ![](dotnetimages/collapse.gif)See Also

####

[IVariableFilletFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVariableFilletFeatureData2_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ISimpleFilletFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISimpleFilletFeatureData2.html)

[IChamferFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChamferFeatureData2.html)