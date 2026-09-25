<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMacroFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IMacroFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to the data that defines a macro feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IMacroFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMacroFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IMacroFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IMacroFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MacroFeatureData.

# ![](dotnetimages/collapse.gif)Example

[Create Macro Feature Subfeature (VBA)](Create_Macro_Feature_Subfeature_Example_VB.htm)

[Cut Body in Half Using Macro Feature (VBA)](Cut_Body_in_Half_using_Macro_Feature_Example_VB.htm)

[Assign Tracking ID Using Macro Feature (VBA)](Assign_Tracking_ID_Using_Macro_Feature_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **Macro features can...** | **For the** **rebuild function** **only, the macro associated with a macro feature cannot:** |
| * be inserted into a part, assembly, or drawing document * create multiple bodies * edit multiple existing bodies | * insert a feature from a macro feature in the same model * edit definitions of other features if these features are in the same model as the macro feature * rebuild, roll back, or roll forward the FeatureManager design tree   NOTE: These limitations are intended to prevent nested-feature regeneration in the model that contains the macro feature. |

When the feature is creating multiple bodies, then the return value from the rebuild function should contain the array of bodies that are the result of the operation. [IMacroFeatureData::EditBodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~EditBodies.html) is not expected to contain a body when the rebuild function returns to SOLIDWORKS.

When the feature is modifying a body and the result is multiple bodies, then IMacroFeatureData::EditBodies should contain all of the resulting bodies.

Whether creating multiple bodies or modifying a body that results in multiple bodies, call [IMacroFeatureData::EnableMultiBodyConsume](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~EnableMultiBodyConsume.html) from the rebuild function to specify whether multiple bodies replace or append the original edit body in the FeatureManager design tree Solid Bodies folder.

If your application allows the user to decide which bodies to keep, your application must determine what it means to select the bodies and subsequently store the selected bodies with the feature.

To edit a macro feature in a drawing, do not use [IMacroFeatureData::AccessSelections](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~AccessSelections.html), [IMacroFeatureData::IAccessSelections](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~IAccessSelections.html),  or [IMacroFeatureData::ReleaseSelectionAccess](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~ReleaseSelectionAccess.html) because the concept of a rollback bar does not exist. You can still use [IFeature::ModifyDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~ModifyDefinition.html) or [IFeature::IModifyDefinition2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~IModifyDefinition2.html) to update an IMacroFeatureData object.

If the user decides to cancel the changes made to the IMacroFeatureData object, then discard the IMacroFeatureData object. This action is equivalent to using IMacroFeatureData::ReleaseSelectionAccess.

See Overview of Macro Features for more information.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[MacroFeatureData](SWObjectModel.pdf#MacroFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[IMacroFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::IInsertMacroFeature3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertMacroFeature3.html)

[IFeatureManager::InsertMacroFeature3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMacroFeature3.html)