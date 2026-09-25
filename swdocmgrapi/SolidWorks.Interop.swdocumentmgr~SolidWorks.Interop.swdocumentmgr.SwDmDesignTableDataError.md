<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.SwDmDesignTableDataError.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| SwDmDesignTableDataError Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) : SwDmDesignTableDataError Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Design table data errors.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum SwDmDesignTableDataError     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As SwDmDesignTableDataError ``` | |

| C# |  |
| --- | --- |
| ``` public enum SwDmDesignTableDataError : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class SwDmDesignTableDataError : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDmDesignTableDataError\_ExternalTableFound** | 0 = The SOLIDWORKS document has an external design table, which is linked to and has been found on disk |
| **swDmDesignTableDataError\_Fail** | 5 = Unknown failure |
| **swDmDesignTableDataError\_InternalTable** | 1 = The SOLIDWORKS document has an internal design table, so there is no external filename |
| **swDmDesignTableDataError\_NoData** | 4 = The SOLIDWORKS document was saved before in a version of SOLIDWORKS earlier than SOLIDWORKS 2009 SP0, so no data is available |
| **swDmDesignTableDataError\_NoTable** | 2 = The SOLIDWORKS document does not have a design table |
| **swDMDesigTableDataError\_ExternalTableNotFound** | 3 = The SOLIDWORKS document has an external design table, but it cannot be found on disk |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html)