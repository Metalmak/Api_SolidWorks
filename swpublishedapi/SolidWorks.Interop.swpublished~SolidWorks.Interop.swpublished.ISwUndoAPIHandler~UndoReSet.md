<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwUndoAPIHandler~UndoReSet.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| UndoReSet Method (ISwUndoAPIHandler) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [ISwUndoAPIHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwUndoAPIHandler.html) : UndoReSet Method (ISwUndoAPIHandler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Resets (clears) the add-in application's undo list after processing the add-in application's undo command and lets an add-in application know that its undo list has been reset.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub UndoReSet() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwUndoAPIHandler   instance.UndoReSet() ``` | |

| C# |  |
| --- | --- |
| ``` void UndoReSet() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void UndoReSet(); ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwUndoAPIHandler::UndoReSet.

# ![](dotnetimages/collapse.gif)Example

[Automate Add-in's Undo Commands (VBA)](Automate_Add-in%27s_Undo_Commands_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISwUndoAPIHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwUndoAPIHandler.html)

[ISwUndoAPIHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwUndoAPIHandler_members.html)