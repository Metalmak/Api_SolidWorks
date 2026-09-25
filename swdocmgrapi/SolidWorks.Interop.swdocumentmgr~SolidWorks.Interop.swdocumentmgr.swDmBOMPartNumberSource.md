<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.swDmBOMPartNumberSource.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| swDmBOMPartNumberSource Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) : swDmBOMPartNumberSource Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sources of bill of materials (BOM) part numbers.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swDmBOMPartNumberSource     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swDmBOMPartNumberSource ``` | |

| C# |  |
| --- | --- |
| ``` public enum swDmBOMPartNumberSource : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swDmBOMPartNumberSource : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDmBOMPartNumber\_ConfigurationName** | 1 |
| **swDmBOMPartNumber\_DocumentName** | 0 |
| **swDmBOMPartNumber\_NotDefined** | -1 = Document was saved in older version of SOLIDWORKS; you must save the document in SOLIDWORKS 2009 or later |
| **swDmBOMPartNumber\_ParentName** | 2 |
| **swDmBOMPartNumber\_UserSpecified** | 3 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html)