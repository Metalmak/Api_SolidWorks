<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_RegenPostNotify2EventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_RegenPostNotify2EventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_RegenPostNotify2EventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*stopFeature*
:   * If rolled back, the [assembly feature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) below the rollback bar in the FeatureManager design tree

    * If rebuilt, Nothing or null

Post-notifies the user program when an assembly document is rebuilt.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_RegenPostNotify2EventHandler( _    ByVal stopFeature As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_RegenPostNotify2EventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_RegenPostNotify2EventHandler(     System.object stopFeature ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_RegenPostNotify2EventHandler(  &   System.Object^ stopFeature ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*stopFeature*
:   * If rolled back, the [assembly feature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html) below the rollback bar in the FeatureManager design tree

    * If rebuilt, Nothing or null

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RegenPostNotify2 Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Assembly Rebuild Events (C#)](Regen_Post_Notify2_Event_Handler_Example_CSharp.htm)

[Fire Assembly Rebuild Events (VB.NET)](Regen_Post_Notify2_Event_Handler_Example_VBNET.htm)

[Fire Assembly Rebuild Events (VBA)](Regen_Post_Notify2_Event_Handler_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAssemblyRegenPostNotify2 to register for this notification.

Use [DAssemblyDocEvents RegenNotifyEventHandler](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_RegenNotifyEventHandler.html) to fire an event before the assembly is about to be rebuilt.

You can also use [IModelDoc2::GetUpdateStamp](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GetUpdateStamp.html) to determine when changes take place in this document.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0