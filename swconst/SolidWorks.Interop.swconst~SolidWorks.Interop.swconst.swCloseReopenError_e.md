<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCloseReopenError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCloseReopenError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCloseReopenError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Close and reopen errors.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCloseReopenError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCloseReopenError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCloseReopenError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCloseReopenError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCloseReopenCloseDocError** | 5; error occurred during close |
| **swCloseReopenInvalidDocError** | 4; document is not a drawing |
| **swCloseReopenLoadFileNotFoundError** | 7; file path specified for document to reopen does not exist |
| **swCloseReopenLoadFilePathEmptyError** | 13; file path of document to reopen is empty |
| **swCloseReopenLoadFilePathNonDrawingError** | 14; file to reopen is not a drawing |
| **swCloseReopenLoadFutureVersionError** | 9; file to reopen is a future version |
| **swCloseReopenLoadGenericError** | 6; error occurred during reopen |
| **swCloseReopenLoadInvalidFileTypeError** | 8; file type is not valid |
| **swCloseReopenLoadLiquidMachineDocError** | 11; LiquidMachine document error |
| **swCloseReopenLoadSameTitleAlreadyOpenError** | 10; file with the same title is already open |
| **swCloseReopenModifiedError** | 12; unable to close the document because changes were made to the document, and [swCloseReopenOption\_e.swCloseReopenOption\_DiscardChanges](SOLIDWORKS.Interop.swconst~SOLIDWORKS.Interop.swconst.swCloseReopenOption_e.html) was not set |
| **swCloseReopenNoError** | 0; no error |
| **swCloseReopenNoInputDocError** | 2; input document is null |
| **swCloseReopenOutputDocPointerError** | 3; output document is null |
| **swCloseReopenUnknownError** | 1; unknown error |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)