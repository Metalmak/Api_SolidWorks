<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~CreateFeatureMgrWindowFromHandlex64.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateFeatureMgrWindowFromHandlex64 Method (IModelViewManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html) : CreateFeatureMgrWindowFromHandlex64 Method (IModelViewManager) |

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

On 64-bit machines, creates a new view in the FeatureManager design tree using the specified .NET tab control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateFeatureMgrWindowFromHandlex64( _    ByVal BitMapFile As System.String, _    ByVal WindowHandle As System.Long, _    ByVal ToolTip As System.String, _    ByVal WhichPane As System.Integer _ ) As FeatMgrView ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelViewManager Dim BitMapFile As System.String Dim WindowHandle As System.Long Dim ToolTip As System.String Dim WhichPane As System.Integer Dim value As FeatMgrView   value = instance.CreateFeatureMgrWindowFromHandlex64(BitMapFile, WindowHandle, ToolTip, WhichPane) ``` | |

| C# |  |
| --- | --- |
| ``` FeatMgrView CreateFeatureMgrWindowFromHandlex64(     System.string BitMapFile,    System.long WindowHandle,    System.string ToolTip,    System.int WhichPane ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` FeatMgrView^ CreateFeatureMgrWindowFromHandlex64(  &   System.String^ BitMapFile, &   System.int64 WindowHandle, &   System.String^ ToolTip, &   System.int WhichPane ) ``` | |

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

See ModelViewManager::CreateFeatureMgrWindowFromHandlex64.

# ![](dotnetimages/collapse.gif)Example

[Add .NET Controls to SOLIDWORKS using an Add-in (C#)](Add_.NET_Controls_to_SOLIDWORKS_Using_an_Add-in_Example_CSharp.htm)

[Add .NET Controls to SOLIDWORKS using an Add-in (VB.NET)](Add_.NET_Controls_to_SolidWorks_Using_an_Add-in_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is only available through early binding and with 64-bit versions of the SOLIDWORKS software.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html)

[IModelViewManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager_members.html)

[IModelViewManager::DisplayWindowFromHandlex64 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~DisplayWindowFromHandlex64.html)

[IModelViewManager::CreateFeatureMgrWindowFromHandle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~CreateFeatureMgrWindowFromHandle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0