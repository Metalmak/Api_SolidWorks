<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_End3DInterconnectTranslationNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_End3DInterconnectTranslationNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_End3DInterconnectTranslationNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Name of imported or exported third-party native CAD file

Notifies the user program when the SOLIDWORKS application is finished importing or exporting a third-party native CAD file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_End3DInterconnectTranslationNotifyEventHandler( _    ByVal FileName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_End3DInterconnectTranslationNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_End3DInterconnectTranslationNotifyEventHandler(     System.string FileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_End3DInterconnectTranslationNotifyEventHandler(  &   System.String^ FileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Name of imported or exported third-party native CAD file

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See End3DInterconnectTranslationNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Example

See the [IImport3DInterconnectData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IImport3DInterconnectData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swAppEnd3DInterconnectTranslationNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2020 FCS, Revision Number 28.0