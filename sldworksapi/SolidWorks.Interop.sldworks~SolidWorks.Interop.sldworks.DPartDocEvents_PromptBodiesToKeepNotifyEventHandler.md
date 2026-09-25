<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_PromptBodiesToKeepNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_PromptBodiesToKeepNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_PromptBodiesToKeepNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Feature*
:   [Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

*Bodies*
:   Array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

Generated when a body is cut into multiple bodies.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_PromptBodiesToKeepNotifyEventHandler( _    ByVal Feature As System.Object, _    ByRef Bodies As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_PromptBodiesToKeepNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_PromptBodiesToKeepNotifyEventHandler(     System.object Feature,    ref System.object Bodies ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_PromptBodiesToKeepNotifyEventHandler(  &   System.Object^ Feature, &   System.Object^% Bodies ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Feature*
:   [Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

*Bodies*
:   Array of [bodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PromptBodiesToKeepNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Example

[Cut Body and Keep All Bodies (C#)](Cut_Body_and_Keep_All_Bodies_Example_CSharp.htm)

[Cut Body and Keep All Bodies (VB.NET)](Cut_Body_and_Keep_All_Bodies_Example_VBNET.htm)

[Cut Body and Keep All Bodies (VBA)](Cut_Body_and_Keep_All_Bodies_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swPartPromptBodiesToKeepNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0