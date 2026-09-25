<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_DragStateChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_DragStateChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_DragStateChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*State*
:   True if dragging of the Instant3D manipulator has started, false if dragging of the Instant3D manipulator has stopped

Fired when starting or stopping the dragging of an Instant3D manipulator.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_DragStateChangeNotifyEventHandler( _    ByVal State As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_DragStateChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_DragStateChangeNotifyEventHandler(     System.bool State ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_DragStateChangeNotifyEventHandler(  &   System.bool State ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*State*
:   True if dragging of the Instant3D manipulator has started, false if dragging of the Instant3D manipulator has stopped

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DragStateChangeNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Events When Dragging Instant3D Manipulator in an Assembly (C#)](Fire_Events_When_Dragging_Instant3D_Manipulator_in_an_Assembly_Example_CSharp.htm)

[Fire Events When Dragging Instant3D Manipulator in an Assembly (VB.NET)](Fire_Events_When_Dragging_Instant3D_Manipulator_in_an_Assembly_Example_VBNET.htm)

[Fire Events When Dragging Instant3D Manipulator in an Assembly (VBA)](Fire_Events_When_Dragging_Instant3D_Manipulator_in_an_Assembly_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAssemblyDragStateChangeNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0