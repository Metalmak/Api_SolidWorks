<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwUndoAPIHandler~DoUndo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| DoUndo Method (ISwUndoAPIHandler) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwUndoAPIHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwUndoAPIHandler.html) : DoUndo Method (ISwUndoAPIHandler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Undoes an add-in application's previously processed commands when an end-user selects its undo command on the SOLIDWORKS undo list or it is called in a macro.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub DoUndo() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwUndoAPIHandler   instance.DoUndo() ``` | |

| C# |  |
| --- | --- |
| ``` void DoUndo() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DoUndo(); ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwUndoAPIHandler::DoUndo.

# ![](dotnetimages/collapse.gif)Example

[Automate Add-in's Undo Commands (VBA)](Automate_Add-in%27s_Undo_Commands_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISwUndoAPIHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwUndoAPIHandler.html)

[ISwUndoAPIHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwUndoAPIHandler_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0