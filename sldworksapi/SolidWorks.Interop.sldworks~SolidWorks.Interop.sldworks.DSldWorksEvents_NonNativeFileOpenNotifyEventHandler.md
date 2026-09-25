<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_NonNativeFileOpenNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_NonNativeFileOpenNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_NonNativeFileOpenNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Name of the opened file

Fired when non-native SOLIDWORKS files are opened.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_NonNativeFileOpenNotifyEventHandler( _    ByVal FileName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_NonNativeFileOpenNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_NonNativeFileOpenNotifyEventHandler(     System.string FileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_NonNativeFileOpenNotifyEventHandler(  &   System.String^ FileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Name of the opened file

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See NonNativeFileOpenNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Remarks

This event occurs after automatic healing if it is enabled. To enable automatic healing, set swImportAutoRunImportDiagnosticsPersist and swImportAutoRunImportDiagnostics to True. See swUserPreferenceToggle\_e, Import for details about these two enumerators.

The file types handled include files with these extensions: .dxf, .dwg, .igs, .sat, .step, .vda, .wrl, and .dll.

On receiving this event, you can call [ISldWorks::ActiveDoc](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~ActiveDoc.html) or [ISldWorks::IActiveDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~IActiveDoc2.html) to get the active [IModelDoc2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2.html) pointer.

In an environment when multiple applications are simultaneously loaded and have access to the SOLIDWORKS application through its APIs, exercise caution when this notification is processed. The active IModelDoc2 may not be the one that corresponds to the FileName argument. For example, this can occur when one of the translator DLL's receives this event and picks up the non-native file and generates a new SOLIDWORKS document. This could happen prior to your application receiving this event.

 If developing a C++ application, use swAppNonNativeFileOpenNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0