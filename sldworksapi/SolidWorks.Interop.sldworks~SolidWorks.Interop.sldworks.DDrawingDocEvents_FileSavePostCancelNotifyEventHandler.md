<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DDrawingDocEvents_FileSavePostCancelNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DDrawingDocEvents\_FileSavePostCancelNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DDrawingDocEvents\_FileSavePostCancelNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Fired if [FileSavePostNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DDrawingDocEvents_FileSavePostNotifyEventHandler.html) is not fired.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DDrawingDocEvents_FileSavePostCancelNotifyEventHandler() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DDrawingDocEvents_FileSavePostCancelNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_FileSavePostCancelNotifyEventHandler() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_FileSavePostCancelNotifyEventHandler(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FileSavePostCancelNotify Event (DrawingDoc).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swDrawingFileSavePostCancelNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0