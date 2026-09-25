<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedSavingDocumentEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| \_IEModelViewControlEvents\_OnFailedSavingDocumentEventHandler Delegate (eDrawings.Interop.EModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) : \_IEModelViewControlEvents\_OnFailedSavingDocumentEventHandler Delegate (eDrawings.Interop.EModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Name of file to save

*ErrorCode*
:   Not used

*ErrorString*
:   Not used

Fired when saving an eDrawings document fails.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Sub _IEModelViewControlEvents_OnFailedSavingDocumentEventHandler( _    ByVal FileName As System.String, _    ByVal ErrorCode As System.Integer, _    ByVal ErrorString As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New _IEModelViewControlEvents_OnFailedSavingDocumentEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnFailedSavingDocumentEventHandler(     System.string FileName,    System.int ErrorCode,    System.string ErrorString ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate void _IEModelViewControlEvents_OnFailedSavingDocumentEventHandler(  &   System.String^ FileName, &   System.int ErrorCode, &   System.String^ ErrorString ) ``` | |

#### Parameters

*FileName*
:   Name of file to save

*ErrorCode*
:   Not used

*ErrorString*
:   Not used

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OnFailedSavingDocument Event (EModelViewControl).

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2006 SP0