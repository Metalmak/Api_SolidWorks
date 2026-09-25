<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~ExpandFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ExpandFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : ExpandFeature Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Component*
:   [Component](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

*FeatureName*
:   Name of a feature in Component

*WhichPane*
:   FeatureManager design tree pane in which to expand Component as defined in swFeatMgrPane\_e

Expands the specified component in the specified FeatureManager design tree pane.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExpandFeature( _    ByVal Component As System.Object, _    ByVal FeatureName As System.String, _    ByVal WhichPane As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Component As System.Object Dim FeatureName As System.String Dim WhichPane As System.Integer Dim value As System.Boolean   value = instance.ExpandFeature(Component, FeatureName, WhichPane) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ExpandFeature(     System.object Component,    System.string FeatureName,    System.int WhichPane ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ExpandFeature(  &   System.Object^ Component, &   System.String^ FeatureName, &   System.int WhichPane ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Component*
:   [Component](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2.html)

*FeatureName*
:   Name of a feature in Component

*WhichPane*
:   FeatureManager design tree pane in which to expand Component as defined in swFeatMgrPane\_e

#### Return Value

True if the specified component is expanded in the specified FeatureManager design tree pane, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::ExpandFeature.

# ![](dotnetimages/collapse.gif)Example

[Expand Component in Specified FeatureManager Design Tree Pane (C#)](Expand_Component_in_Specified_FeatureManager_Design_Tree_Pane_Example_CSharp.htm)

[Expand Component in Specified FeatureManager Design Tree Pane (VB.NET)](Expand_Component_in_Specified_FeatureManager_Design_Tree_Pane_Example_VBNET.htm)

[Expand Component in Specified FeatureManager Design Tree Pane (VBA)](Expand_Component_in_Specified_FeatureManager_Design_Tree_Pane_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ITreeControlItem::Expanded Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITreeControlItem~Expanded.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0