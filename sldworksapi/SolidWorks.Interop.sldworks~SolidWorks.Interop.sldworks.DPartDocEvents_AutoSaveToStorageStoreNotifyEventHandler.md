<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_AutoSaveToStorageStoreNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_AutoSaveToStorageStoreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_AutoSaveToStorageStoreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Fired when the part document is automatically saved to third-party IStorage storage.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_AutoSaveToStorageStoreNotifyEventHandler() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_AutoSaveToStorageStoreNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_AutoSaveToStorageStoreNotifyEventHandler() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_AutoSaveToStorageStoreNotifyEventHandler(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AutoSaveToStorageStoreNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAutoSaveToStorageStoreNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0