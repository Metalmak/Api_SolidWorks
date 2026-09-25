<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedPrintingDocumentEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnFailedPrintingDocumentEventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnFailedPrintingDocumentEventHandler Delegate (eDrawings.Interop.EModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PrintJobName*
:   String specified for the FileNameInPrintQueue argument in [IEModelViewControl::Print5](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Print5.html) or an empty string if the ShowDialog argument of IEModelViewControl::Print5 was set to true and the user prints from the user interface

Fired if the printer name specified in the [IEModelViewControl::SetPageSetupOptions](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~SetPageSetupOptions.html) was invalid or if an eDrawings-related error exists that prevents data from being sent to a printer queue.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnFailedPrintingDocumentEventHandler( _    ByVal PrintJobName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnFailedPrintingDocumentEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnFailedPrintingDocumentEventHandler(     System.string PrintJobName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnFailedPrintingDocumentEventHandler(  &   System.String^ PrintJobName ) ``` | |

#### Parameters

*PrintJobName*
:   String specified for the FileNameInPrintQueue argument in [IEModelViewControl::Print5](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Print5.html) or an empty string if the ShowDialog argument of IEModelViewControl::Print5 was set to true and the user prints from the user interface

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OnFailedPrintingDocument Event (EModelViewControl).

# ![](dotnetimages/collapse.gif)Remarks

When this event is fired, eDrawings has sent all of the eDrawings data in the active document to the printer queue, and it is safe to close the active document or open another one.

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2006 SP0