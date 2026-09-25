<!-- source: toolboxapi/SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser.swPDMDocManagerEvents_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| swPDMDocManagerEvents\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html) : swPDMDocManagerEvents\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Events to be handled by the PDM application.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPDMDocManagerEvents_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPDMDocManagerEvents_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPDMDocManagerEvents_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPDMDocManagerEvents_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAfterCopyingDocument** | 9 = Notifies after Toolbox Browser copies or moves a PDM document |
| **swAfterDeletingDocument** | 7 = Notifies after Toolbox Browser deletes a PDM document |
| **swAfterWritingToDocument** | 3 = Notifies after Toolbox Browser writes to a PDM document |
| **swBeforeCopyingDocument** | 8 = Notifies before Toolbox Browser copies or moves a PDM document |
| **swBeforeDeletingDocument** | 6 = Notifies before Toolbox Browser deletes a PDM document |
| **swBeforeWritingToDocument** | 2 = Notifies before Toolbox Browser writes to a PDM document |
| **swNewDocumentAdded** | 5 = Notifies that Toolbox Browser has created a new PDM document or added a PDM document to the Toolbox Browser |
| **swPDMDestroy** | 1 = Notifies that the PDM application object is being destroyed |
| **swPreInsertDocument** | 4 = Notifies before Toolbox Browser inserts a PDM document into an assembly |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swbrowser Namespace](SolidWorks.Interop.swbrowser~SolidWorks.Interop.swbrowser_namespace.html)