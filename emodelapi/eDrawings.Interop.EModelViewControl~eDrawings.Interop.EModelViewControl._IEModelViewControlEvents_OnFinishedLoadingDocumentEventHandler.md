<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedLoadingDocumentEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnFinishedLoadingDocumentEventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnFinishedLoadingDocumentEventHandler Delegate (eDrawings.Interop.EModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Name of document being opened

Fired when the eDrawings file has finished loading.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnFinishedLoadingDocumentEventHandler( _    ByVal FileName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnFinishedLoadingDocumentEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnFinishedLoadingDocumentEventHandler(     System.string FileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnFinishedLoadingDocumentEventHandler(  &   System.String^ FileName ) ``` | |

#### Parameters

*FileName*
:   Name of document being opened

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OnFinishedLoadingDocument Event (EModelViewControl).

# ![](dotnetimages/collapse.gif)Remarks

Because [IEModelViewControl::OpenDoc](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~OpenDoc.html) starts a new thread of execution and because eDrawings files are often loaded across the Internet or other potentially slow and unreliable networks, this API call can return before the document is finished loading.

Referencing a model that has not finished loading (for example, calling [IEModelViewControl::Animate](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Animate.html)) can cause your application to hang, crash, or behave unpredictably. Therefore, listen for the OnFinishedLoadingDocument event after calling IEModelViewControl::OpenDoc so that your application knows when the eDrawings file is finished loading. Once your application receives notification that the eDrawings file has been loaded, it is safe to access the model.

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0