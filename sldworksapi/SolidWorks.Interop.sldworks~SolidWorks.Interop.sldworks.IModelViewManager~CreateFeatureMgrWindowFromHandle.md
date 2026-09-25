<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~CreateFeatureMgrWindowFromHandle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFeatureMgrWindowFromHandle Method (IModelViewManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html) : CreateFeatureMgrWindowFromHandle Method (IModelViewManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BitMapFile*
:   Fully qualified path to the bitmap file that you want to use for the control

*WindowHandle*
:   Handle of the .NET tab control

*ToolTip*
:   Text for the ToolTip

*WhichPane*
:   Pane to use as defined in swFeatMgrPane\_e

Creates a new view in the FeatureManager design tree using the specified .NET tab control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFeatureMgrWindowFromHandle( _    ByVal BitMapFile As System.String, _    ByVal WindowHandle As System.Integer, _    ByVal ToolTip As System.String, _    ByVal WhichPane As System.Integer _ ) As FeatMgrView ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelViewManager Dim BitMapFile As System.String Dim WindowHandle As System.Integer Dim ToolTip As System.String Dim WhichPane As System.Integer Dim value As FeatMgrView   value = instance.CreateFeatureMgrWindowFromHandle(BitMapFile, WindowHandle, ToolTip, WhichPane) ``` | |

| C# |  |
| --- | --- |
| ``` FeatMgrView CreateFeatureMgrWindowFromHandle(     System.string BitMapFile,    System.int WindowHandle,    System.string ToolTip,    System.int WhichPane ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` FeatMgrView^ CreateFeatureMgrWindowFromHandle(  &   System.String^ BitMapFile, &   System.int WindowHandle, &   System.String^ ToolTip, &   System.int WhichPane ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BitMapFile*
:   Fully qualified path to the bitmap file that you want to use for the control

*WindowHandle*
:   Handle of the .NET tab control

*ToolTip*
:   Text for the ToolTip

*WhichPane*
:   Pane to use as defined in swFeatMgrPane\_e

#### Return Value

[IFeatMgrView](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatMgrView.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelViewManager::CreateFeatureMgrWindowFromHandle.

# ![](dotnetimages/collapse.gif)Remarks

If your application must be x64 compatible, then use [IModelViewManager::CreateFeatureMgrWindowFromHandlex64](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelViewManager~CreateFeatureMgrWindowFromHandlex64.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html)

[IModelViewManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager_members.html)

[IModelViewManager::DisplayWindowFromHandle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~DisplayWindowFromHandle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0