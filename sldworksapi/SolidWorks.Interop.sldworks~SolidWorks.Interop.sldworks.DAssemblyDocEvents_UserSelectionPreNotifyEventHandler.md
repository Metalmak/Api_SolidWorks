<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_UserSelectionPreNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_UserSelectionPreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_UserSelectionPreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SelType*
:   Type of object to be selected as defined by swSelectType\_e

Fired when an interactive user moves the cursor over or clicks a model view in an assembly document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_UserSelectionPreNotifyEventHandler( _    ByVal SelType As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_UserSelectionPreNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_UserSelectionPreNotifyEventHandler(     System.int SelType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_UserSelectionPreNotifyEventHandler(  &   System.int SelType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SelType*
:   Type of object to be selected as defined by swSelectType\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See UserSelectionPreNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Disable Selection of Faces and Edges Using a Pre-Notify Event (VBA)](Disable_Selection_of_Faces_and_Edges_Using_a_Pre-Notify_Event_Example_VB.htm)

[Disable Selection of Faces and Edges Using a Pre-Notify Event (VB.NET)](Disable_Selection_of_Faces_and_Edges_Using_a_Pre-Notify_Event_Example_VBNET.htm)

[Disable Selection of Faces and Edges Using a Pre-Notify Event (C#)](Disable_Selection_of_Faces_and_Edges_Using_a_Pre-Notify_Event_Example_CSharp.htm)

[Get Preselected Object (C#)](Get_Preselected_Object_Example_CSharp.htm)

[Get Preselected Object (VB.NET)](Get_Preselected_Object_Example_VBNET.htm)

[Get Preselected Object (VBA)](Get_Preselected_Object_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Only selections made interactively fire this event; selections made programmatically are ignored by this event.

If developing a C++ application, use swAssemblyUserSelectionPreNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0