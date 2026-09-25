<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_FileOpenPreNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_FileOpenPreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_FileOpenPreNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Full path and name of file to open

Pre-notifies the user program of a [FileOpenNotify2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_FileOpenNotify2EventHandler.html) event.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_FileOpenPreNotifyEventHandler( _    ByVal FileName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_FileOpenPreNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_FileOpenPreNotifyEventHandler(     System.string FileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_FileOpenPreNotifyEventHandler(  &   System.String^ FileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Full path and name of file to open

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FileOpenPreNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Remarks

This event is only fired when opening these SOLIDWORKS files: parts, drawings, and assemblies. It is not fired when opening files like templates, translator files, and so on.

This event is fired before SOLIDWORKS begins loading the file. A SOLIDWORKS file can be opened in many ways; for example, File, Open in the user interface, [ISldWorks::OpenDoc6](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~OpenDoc6.html) in the API, Load Model from a Detached drawing, Lightweight component being resolved, and so on. This event is fired in all of these cases.

If you want to allow SOLIDWORKS to open the file, return S\_OK (or 0) from the handler. If you do not want to allow SOLIDWORKS to open the file, return S\_false (or any code other than S\_OK) from the handler.

The event that occurs after this event is [DocumentLoadNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_DocumentLoadNotifyEventHandler.html).

If developing a C++ application, use swAppFileOpenPreNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 SP4, Revision Number 12.4