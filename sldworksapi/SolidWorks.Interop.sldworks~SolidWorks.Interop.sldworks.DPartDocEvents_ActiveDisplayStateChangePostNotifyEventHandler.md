<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_ActiveDisplayStateChangePostNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_ActiveDisplayStateChangePostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_ActiveDisplayStateChangePostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DisplayStateName*
:   Name of the active display state

Fired after the display state of a configuration is changed or after a configuration is changed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_ActiveDisplayStateChangePostNotifyEventHandler( _    ByVal DisplayStateName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_ActiveDisplayStateChangePostNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_ActiveDisplayStateChangePostNotifyEventHandler(     System.string DisplayStateName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_ActiveDisplayStateChangePostNotifyEventHandler(  &   System.String^ DisplayStateName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*DisplayStateName*
:   Name of the active display state

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ActiveDisplayStateChangePostNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Events When Display State Changes in Part Document (C#)](Fire_Events_When_Display_State_Changes_in_Part_Document_Example_CSharp.htm)

[Fire Events When Display State Changes in Part Document (VB.NET)](Fire_Events_When_Display_State_Changes_in_Part_Document_Example_VBNET.htm)

[Fire Events When Display State Changes in Part Document (VBA)](Fire_Events_When_Display_State_Changes_in_Part_Document_Example_VB6.htm)

# ![](dotnetimages/collapse.gif)Remarks

When changing configurations, the following events are fired in this order:

* [ActiveConfigChangeNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DPartDocEvents_ActiveConfigChangeNotifyEventHandler.html)* [ActiveDisplayStateChangePreNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DPartDocEvents_ActiveDisplayStateChangePreNotifyEventHandler.html)* [ActiveConfigChangePostNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DPartDocEvents_ActiveConfigChangePostNotifyEventHandler.html)* ActiveDisplayStateChangePostNotify

When changing the display state of a configuration, only ActiveDisplayStateChangePreNotify and ActiveDisplayStateChangePostNotify are fired.

This event is fired even when configurations and display states are not linked; however, the initial and final display states will be the same.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 17.0