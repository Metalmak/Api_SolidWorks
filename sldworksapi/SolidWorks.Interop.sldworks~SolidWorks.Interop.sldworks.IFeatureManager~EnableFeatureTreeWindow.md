<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~EnableFeatureTreeWindow.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EnableFeatureTreeWindow Property (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : EnableFeatureTreeWindow Property (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether the FeatureManager design tree is enabled or not.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EnableFeatureTreeWindow As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim value As System.Boolean   instance.EnableFeatureTreeWindow = value   value = instance.EnableFeatureTreeWindow ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EnableFeatureTreeWindow {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool EnableFeatureTreeWindow {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::EnableFeatureTreeWindow.

# ![](dotnetimages/collapse.gif)Remarks

Use this property with [IFeatureManager::EnableFeatureTree](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~EnableFeatureTree.html), which temporarily enables or disables the FeatureManager design tree update when an add-in is running a series of operations.

While the FeatureManager design tree is disabled and not being updated, the FeatureManager tree may become out of date with what is actually in the model. If an interactive user attempts to interact with the FeatureManager design tree while it is in this out-of-date state, problems could occur. Normally, this should not happen because the add-in should only be disabling the FeatureManager design tree update temporarily and then enabling it immediately after the series of operations complete. However, if there is any possibility that an interactive user could interact with the FeatureManager design tree, then use FeatureManager::EnableFeatureTreeWindow, which prohibits any user interaction with the FeatureManager design tree because the control is disabled.

Just as with the IFeatureManager::EnableFeatureTree property, this property is meant to be used for temporary disabling. If it is necessary to disable the FeatureManager design tree control, then it should only be disabled while the add-in is performing some series of operations and enabled immediately after these operations complete. Do not to leave the FeatureManager design tree window disabled when control is returned to SOLIDWORKS, i.e., the interactive user.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::UpdateFeatureTree Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~UpdateFeatureTree.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 SP2, Revision Number 13.2