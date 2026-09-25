<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_RenameDisplayTitleNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_RenameDisplayTitleNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_RenameDisplayTitleNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*oldName*
:   Previous display title

*NewName*
:   New display title

Fired when the display title changes for an item in the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_RenameDisplayTitleNotifyEventHandler( _    ByVal oldName As System.String, _    ByVal NewName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_RenameDisplayTitleNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_RenameDisplayTitleNotifyEventHandler(     System.string oldName,    System.string NewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_RenameDisplayTitleNotifyEventHandler(  &   System.String^ oldName, &   System.String^ NewName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*oldName*
:   Previous display title

*NewName*
:   New display title

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenameDisplayTitleNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Remarks

Change the display title by using [IModelDocExtension::DisplayTitle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DisplayTitle.html).

If developing a C++ application, use swAssemblyRenamedDisplayTitleNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 SP4, Revision Number 28.4