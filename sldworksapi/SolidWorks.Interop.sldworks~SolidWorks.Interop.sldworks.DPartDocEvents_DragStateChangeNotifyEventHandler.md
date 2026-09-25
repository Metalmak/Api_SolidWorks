<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_DragStateChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_DragStateChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_DragStateChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*State*
:   True if dragging of the Instant3D manipulator has started; false if dragging of the Instant3D manipulator has stopped

Fired when starting or stopping the dragging of an Instant3D manipulator.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_DragStateChangeNotifyEventHandler( _    ByVal State As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_DragStateChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_DragStateChangeNotifyEventHandler(     System.bool State ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_DragStateChangeNotifyEventHandler(  &   System.bool State ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*State*
:   True if dragging of the Instant3D manipulator has started; false if dragging of the Instant3D manipulator has stopped

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DragStateChangeNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Events When Dragging Instant3D Manipulator in a Part (C#)](Fire_Events_When_Dragging_Instant3D_Manipulator_in_a_Part_Example_CSharp.htm)

[Fire Events When Dragging Instant3D Manipulator in a Part (VB.NET)](Fire_Events_When_Dragging_Instant3D_Manipulator_in_a_Part_Example_VBNET.htm)

[Fire Events When Dragging Instant3D Manipulator in a Part (VBA)](Fire_Events_When_Dragging_Instant3D_Manipulator_in_a_Part_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swPartDragStateChangeNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0