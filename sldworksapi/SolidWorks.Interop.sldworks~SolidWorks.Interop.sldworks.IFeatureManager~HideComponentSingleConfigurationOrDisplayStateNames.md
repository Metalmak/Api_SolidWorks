<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~HideComponentSingleConfigurationOrDisplayStateNames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| HideComponentSingleConfigurationOrDisplayStateNames Property (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : HideComponentSingleConfigurationOrDisplayStateNames Property (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to hide a component's only configuration or display state.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property HideComponentSingleConfigurationOrDisplayStateNames As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim value As System.Boolean   instance.HideComponentSingleConfigurationOrDisplayStateNames = value   value = instance.HideComponentSingleConfigurationOrDisplayStateNames ``` | |

| C# |  |
| --- | --- |
| ``` System.bool HideComponentSingleConfigurationOrDisplayStateNames {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool HideComponentSingleConfigurationOrDisplayStateNames {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to hide the single configuration or display state, false to display it

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::HideComponentSingleConfigurationOrDisplayStateNames.

# ![](dotnetimages/collapse.gif)Example

See the [IFeatureManager::SetComponentIdentifiers](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetComponentIdentifiers.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This property:

* Works in both SOLIDWORKS Desktop and SOLIDWORKS Connected.* Is analogous to the **Do not show Configuration or Display State name if only one exists** check box on the Component Name and Description dialog that appears after right-clicking on the top-level component in the FeatureManager design tree and selecting **Tree Display > Component Name and Description**.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 SP01, Revision Number 30.1