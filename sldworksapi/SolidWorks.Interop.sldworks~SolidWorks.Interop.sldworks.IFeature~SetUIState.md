<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~SetUIState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetUIState Method (IFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) : SetUIState Method (IFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StateType*
:   User interface state type as defined in swUIStates\_e

*Flag*
:   True to set the user-interface state, false to not

Sets the user-interface state of the current feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetUIState( _    ByVal StateType As System.Integer, _    ByVal Flag As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeature Dim StateType As System.Integer Dim Flag As System.Boolean   instance.SetUIState(StateType, Flag) ``` | |

| C# |  |
| --- | --- |
| ``` void SetUIState(     System.int StateType,    System.bool Flag ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetUIState(  &   System.int StateType, &   System.bool Flag ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StateType*
:   User interface state type as defined in swUIStates\_e

*Flag*
:   True to set the user-interface state, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Feature::SetUIState.

# ![](dotnetimages/collapse.gif)Example

[Display of Item in FeatureManager Design Tree (C++)](Display_of_Item_in_Feature_Manager_Example_CPlusPlus_COM.htm)

[Hide Feature in FeatureManager Design Tree (VBA)](Hide_Feature_in_FeatureManager_Design_Tree_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If you pass in StateType of swIsHiddenInFeatureMgr and flag of True, then this method hides the display of the feature in the FeatureManager design tree. To see your changes in the FeatureManager design tree , use [IModelDoc2::EditRebuild3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~EditRebuild3.html).

Features are initialized with all user-interface state type values set to false. However, in the case of attributes, you can use [IAttributeDef::CreateInstance5](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAttributeDef~CreateInstance5.html) to set the desired display state of the attribute at the time of creation.

A change in a the state setting of a feature causes all its dependents to inherit the same behavior, without actually setting the state type values of those dependents. Therefore, to get the actual user-interface state value of a feature, you can query its owner.

The user-interface state is not a property.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeature Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

[IFeature Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature_members.html)

[IFeature::Visible Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~Visible.html)

[IFeature::GetUIState Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetUIState.html)