<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~DisplayWindowFromHandle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DisplayWindowFromHandle Method (IModelViewManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html) : DisplayWindowFromHandle Method (IModelViewManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   User-defined label that appears on the tab

*WindowHandle*
:   Handle of the .NET control

*SplitWindow*
:   True to add a splitter window, false to not

Displays a .NET control in this model view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DisplayWindowFromHandle( _    ByVal Name As System.String, _    ByVal WindowHandle As System.Integer, _    ByVal SplitWindow As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelViewManager Dim Name As System.String Dim WindowHandle As System.Integer Dim SplitWindow As System.Boolean Dim value As System.Boolean   value = instance.DisplayWindowFromHandle(Name, WindowHandle, SplitWindow) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DisplayWindowFromHandle(     System.string Name,    System.int WindowHandle,    System.bool SplitWindow ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DisplayWindowFromHandle(  &   System.String^ Name, &   System.int WindowHandle, &   System.bool SplitWindow ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   User-defined label that appears on the tab

*WindowHandle*
:   Handle of the .NET control

*SplitWindow*
:   True to add a splitter window, false to not

#### Return Value

True if .NET control is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelViewManager::DisplayWindowFromHandle.

# ![](dotnetimages/collapse.gif)Remarks

If your application must be x64 compatible, then use [IModelViewManager::DisplayWindowFromHandlex64](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelViewManager~DisplayWindowFromHandlex64.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelViewManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager.html)

[IModelViewManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager_members.html)

[IModelViewManager::CreateFeatureMgrWindowFromHandle Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelViewManager~CreateFeatureMgrWindowFromHandle.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0