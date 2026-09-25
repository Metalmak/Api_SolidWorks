<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_FileSavePostNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_FileSavePostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_FileSavePostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*saveType*
:   Type of save as defined in swFileSaveTypes\_e

*FileName*
:   Saved file name

Post-notifies the user program when a part document is saved.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_FileSavePostNotifyEventHandler( _    ByVal saveType As System.Integer, _    ByVal FileName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_FileSavePostNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_FileSavePostNotifyEventHandler(     System.int saveType,    System.string FileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_FileSavePostNotifyEventHandler(  &   System.int saveType, &   System.String^ FileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*saveType*
:   Type of save as defined in swFileSaveTypes\_e

*FileName*
:   Saved file name

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FileSavePostNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swPartFileSavePostNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0