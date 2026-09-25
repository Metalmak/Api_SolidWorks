<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swBlockingStates_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swBlockingStates\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swBlockingStates\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Blocking states.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swBlockingStates_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swBlockingStates_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swBlockingStates_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swBlockingStates_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swEditorBlock** | 4 = A valid return value for IModelDoc2::GetBlockingState, but it is not a valid input for IModelDoc2::SetBlockingState; editing or inserting blocks are blocked |
| **swEditSketchAllowExitBlock** | 8 = Block model changes but allow sketching and exiting sketch edit mode |
| **swEditSketchBlock** | 5 = A block is being edited in the drawing |
| **swFullBlock** | 1 = Most actions are blocked; you cannot edit features, add features, change views (rotate, pan, and so on), exit the SOLIDWORKS software, or change a document; however, you can open a document |
| **swModifyBlock** | 2 = Similar to swFullBlock except that view-related (rotate, pan, and so on) operations are not blocked |
| **swNoBlock** | 0 = No actions are blocked |
| **swPartialModifyBlock** | 3 = Similar to swModifyBlock except that you can change documents |
| **swSystemBlock** | 6 = Similar to swFullBlock except that you cannot open a document |
| **swViewOnlyBlock** | 7 = A valid return value for IModelDoc2::GetBlockingState when a document is open in View only/Selective open mode; not a valid input for IModelDoc2::SetBlockingState |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)