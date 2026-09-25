<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedPrintingDocumentEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnFinishedPrintingDocumentEventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnFinishedPrintingDocumentEventHandler Delegate (eDrawings.Interop.EModelViewControl) |

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

Fired when an eDrawings document finishes printing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnFinishedPrintingDocumentEventHandler( _    ByVal PrintJobName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnFinishedPrintingDocumentEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnFinishedPrintingDocumentEventHandler(     System.string PrintJobName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnFinishedPrintingDocumentEventHandler(  &   System.String^ PrintJobName ) ``` | |

#### Parameters

*PrintJobName*
:   String specified for the FileNameInPrintQueue argument in [IEModelViewControl::Print5](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Print5.html) or an empty string if the ShowDialog argument of IEModelViewControl::Print5 was set to true and the user prints from the user interface

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OnFinishedPrintingDocument Event (EModelViewControl).

# ![](dotnetimages/collapse.gif)Remarks

When this event is fired, eDrawings has sent all of the eDrawings data in the active document to the printer queue, and it is safe to close the active document or open another one.

This event does not guarantee that printing of the eDrawings document was successful. For example, if the printer is out of paper, eDrawings still fires this event and not [OnFailedPrintingDocument](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedPrintingDocumentEventHandler.html).

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2006 SP0