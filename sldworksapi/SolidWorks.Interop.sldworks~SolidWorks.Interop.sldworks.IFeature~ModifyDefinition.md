<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ModifyDefinition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ModifyDefinition Method (IFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : ModifyDefinition Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Data*
:   Feature data object

*TopDoc*
:   Top-level document (see **Remarks**)

*Component*
:   Component for the feature (see Remarks)

Updates the definition of a feature with the new values in an associated feature data object obtained with [IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ModifyDefinition( _    ByVal Data As System.Object, _    ByVal TopDoc As System.Object, _    ByVal Component As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim Data As System.Object Dim TopDoc As System.Object Dim Component As System.Object Dim value As System.Boolean   value = instance.ModifyDefinition(Data, TopDoc, Component) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ModifyDefinition(     System.object Data,    System.object TopDoc,    System.object Component ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ModifyDefinition(  &   System.Object^ Data, &   System.Object^ TopDoc, &   System.Object^ Component ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Data*
:   Feature data object

*TopDoc*
:   Top-level document (see **Remarks**)

*Component*
:   Component for the feature (see Remarks)

#### Return Value

True if the feature definition modified successfully, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Feature::ModifyDefinition.

# ![](dotnetimages/collapse.gif)Example

[Change Bend Radius of Sheet Metal Part (VBA)](Change_Bend_Radius_of_Sheet_Metal_Part_Example_VB.htm)

[Get and Set Constraint for Dome Feature (VBA)](Get_and_Set_Constraint_for_Dome_Feature_Example_VB.htm)

[Modify Plane By Editing its Definition (VBA)](Modify_Plane_by_Editing_Its_Definition_Example_VB.htm)

[Insert and Change DeleteFace Feature (C#)](Insert_and_Change_DeleteFace_Feature_Example_CSharp.htm)

[Insert and Change DeleteFace Feature (VB.NET)](Insert_and_Change_DeleteFace_Feature_Example_VBNET.htm)

[Insert and Change DeleteFace Feature (VBA)](Insert_and_Change_DeleteFace_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If this method returns:

* False, you may have specified invalid properties in the feature data modifier object. The feature definition was not modified, so the feature may have rolled back to its previous state.* True, the feature was updated using the feature data modifier object provided. This method will return true even if the feature data modifier object does not include any changed properties or references; some feature data modifier objects reject invalid changes before this method is called. For some feature modifications, this method applies the new properties, returns true, but results in a new rebuild error on the feature.

In either case, this method may leave the feature in an unpredictable state due to errors. After calling this method, call [IFeature::GetErrorCode2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetErrorCode2.html) to ascertain whether the feature has rebuild errors. If so, try again with valid feature data. To correct rebuild errors, call [IModelDoc2::ForceRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ForceRebuild3.html). You can also move the rollback bar in the FeatureManager design tree to before and after the feature to correct its state.

You should carefully read specific feature data interface documentation to learn how to correctly specify feature data properties and how this method works with specific features.

| **To modify a feature in...** | **Then TopDoc argument...** |
| --- | --- |
| A part | Is the [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) object for the part and the Component argument should be Nothing or null |
| An assembly | Should be the assembly IModelDoc2 object and the Component argument should be the [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) object in which the feature is to be modified |

When you modify a feature in an assembly, this method leaves the assembly in Editing Part mode. You can switch back to editing the assembly by calling [IAssemblyDoc::EditAssembly](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~EditAssembly.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

[IFeature::IGetDefinition Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IGetDefinition.html)

[IFeature::IModifyDefinition2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~IModifyDefinition2.html)