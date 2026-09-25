<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_SelectiveOpenPostNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_SelectiveOpenPostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_SelectiveOpenPostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NewAddedDisplayStateName*
:   Name of the new display state

*SelectedComponentNames*
:   Array of selected component names

Post-notifies the user program when assembly components are selected for Quick View/Selective Open.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_SelectiveOpenPostNotifyEventHandler( _    ByVal NewAddedDisplayStateName As System.String, _    ByRef SelectedComponentNames As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_SelectiveOpenPostNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_SelectiveOpenPostNotifyEventHandler(     System.string NewAddedDisplayStateName,    ref System.object SelectedComponentNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_SelectiveOpenPostNotifyEventHandler(  &   System.String^ NewAddedDisplayStateName, &   System.Object^% SelectedComponentNames ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NewAddedDisplayStateName*
:   Name of the new display state

*SelectedComponentNames*
:   Array of selected component names

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SelectiveOpenPostNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Selective Open Post-Notify Event (VBA)](Selective_Open_Post_Notify_Event_Example_VB.htm)

[Selective Open Post-Notify Event (VB.NET)](Selective_Open_Post_Notify_Event_Example_VBNET.htm)

[Selective Open Post-Notify Event (C#)](Selective_Open_Post_Notify_Event_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAssemblySelectiveOpenPostNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0