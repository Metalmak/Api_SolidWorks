<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_CommandCloseNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_CommandCloseNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_CommandCloseNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Command*
:   Command as defined in swCommands\_e

*reason*
:   Reason as defined in swPropertyManagerPageCloseReasons\_e

Fired when a command, including a PropertyManager page, is okay'd or canceled by a user.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_CommandCloseNotifyEventHandler( _    ByVal Command As System.Integer, _    ByVal reason As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_CommandCloseNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_CommandCloseNotifyEventHandler(     System.int Command,    System.int reason ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_CommandCloseNotifyEventHandler(  &   System.int Command, &   System.int reason ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Command*
:   Command as defined in swCommands\_e

*reason*
:   Reason as defined in swPropertyManagerPageCloseReasons\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CommandCloseNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Example

[Fire Events When PropertyManager Page Opened and Canceled (VBA)](Fire_Events_When_PropertyManager_Page_Opened_and_Canceled_Example_VB.htm)

[Fire Events When PropertyManager Page Opened and Canceled (VB.NET)](Fire_Events_When_PropertyManager_Page_Opened_and_Canceled_Example_VBNET.htm)

[Fire Events When PropertyManager Page Opened and Canceled (C#)](Fire_Events_When_PropertyManager_Page_Opened_and_Canceled_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAppCommandCloseNotify to register for this notification.

You can combine:

* the IAssemblyDoc [FeatureEditPreNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DAssemblyDocEvents_FeatureEditPreNotifyEventHandler.html) event or the IPartDoc [FeatureEditPreNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DPartDocEvents_EquationEditorPreNotifyEventHandler.html) event with the ISldWorks CommandCloseNotify event and swCommands\_e.swCommands\_EditFeature.

  * the IAssemblyDoc [FeatureSketchEditPreNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DAssemblyDocEvents_FeatureSketchEditPreNotifyEventHandler.html) event or the IPartDoc [FeatureSketchEditPreNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DPartDocEvents_FeatureSketchEditPreNotifyEventHandler.html) event with the ISldWorks CommandCloseNotify event and swCommands\_e.swCommands\_Sketch.

Call [CommandOpenPreNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_CommandOpenPreNotifyEventHandler.html) to fire an event before a command executes or a PropertyManager page opens.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0