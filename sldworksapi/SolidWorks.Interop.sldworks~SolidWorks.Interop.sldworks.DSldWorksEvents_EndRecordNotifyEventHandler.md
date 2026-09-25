<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_EndRecordNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_EndRecordNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_EndRecordNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Notifies the user program when a macro recording has ended, including if the user cancels the recording (i.e., the user cancels out of the Save As dialog and says No to the SOLIDWORKS Continue recording? dialog).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_EndRecordNotifyEventHandler() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_EndRecordNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_EndRecordNotifyEventHandler() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_EndRecordNotifyEventHandler(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EndRecordNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Example

[Record Macros (C#)](Record_Macros_Example_CSharp.htm)

[Record Macros (VB.NET)](Record_Macros_Example_VBNET.htm)

[Record Macros (VBA)](Record_Macros_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This event informs the user program when a macro recording has stopped so that the add-in can add its own cleanup code to a macro using [ISldWorks::RecordLine](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RecordLine.html), [ISldWorks::RecordLineCSharp](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RecordLineCSharp.html), or [ISldWorks::RecordLineVBnet](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~RecordLineVBnet.html). This is useful if the add-in has been recording its own lines of code to the macro and needs to clean up variables that have been used.

The SOLIDWORKS event [BeginRecordNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_BeginRecordNotifyEventHandler.html) is sent when the macro recording is starting.

These events are not sent when the macro is paused and restarted. SldWorks::RecordLine, ISldWorks::RecordLineCSharp, or ISldWorks::RecordLineVBnet can be used at any time, regardless of whether a macro is currently recording or not. Even if no macro is running, writing to the journal file occurs.

If developing a C++ application, use swAppEndRecordNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0