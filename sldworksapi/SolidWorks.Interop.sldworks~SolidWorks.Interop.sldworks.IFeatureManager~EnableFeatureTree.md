<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~EnableFeatureTree.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EnableFeatureTree Property (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : EnableFeatureTree Property (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether or not to update the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EnableFeatureTree As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim value As System.Boolean   instance.EnableFeatureTree = value   value = instance.EnableFeatureTree ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EnableFeatureTree {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool EnableFeatureTree {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to update FeatureManager design tree, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::EnableFeatureTree.

# ![](dotnetimages/collapse.gif)Example

[Only Show Selected Components (VBA)](Only_Show_Selected_Components_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use this property to temporarily enable or disable the FeatureManager design tree while an add-in is running a series of operations. Temporarily disabling the FeatureManager design tree should increase performance. However, while the FeatureManager design tree is disabled and not being updated, it may become out of date with what is actually in the model.

If an interactive user attempts to interact with the FeatureManager design tree while it is in this out-of-date state, problems could occur. Normally, this should not happen because the add-in should only be disabling the FeatureManager design tree update temporarily and then enabling it immediately after the series of operations completes. However, if there is any possibility that the interactive user could interact with the FeatureManager design tree while it is an out-of-date state, then also use [IFeatureManager::EnableFeatureTreeWindow](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~EnableFeatureTreeWindow.html), which prohibits any user interaction with the FeatureManager design tree because the control itself is disabled.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::UpdateFeatureTree Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~UpdateFeatureTree.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0