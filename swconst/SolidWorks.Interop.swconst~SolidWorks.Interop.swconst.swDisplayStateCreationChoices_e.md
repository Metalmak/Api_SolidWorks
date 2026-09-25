<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swDisplayStateCreationChoices_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swDisplayStateCreationChoices\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swDisplayStateCreationChoices\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Display-state preserve options.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swDisplayStateCreationChoices_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swDisplayStateCreationChoices_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swDisplayStateCreationChoices_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swDisplayStateCreationChoices_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDisplayStateCreation\_AskUser** | -1; Display the dialog where the user can select the display states (PhotoWorks material and SOLIDWORKS colors) he or she wants to preserve; however, if **swDisplayStateCreation\_AskUser** is set and the user opens the file using **ISldWorks::OpenDoc***n* (where *n* is the version number of the method), then both display states are preserved and the dialog is not displayed; valid in documents created in SOLIDWORKS 2009 and earlier |
| **swDisplayStateCreation\_BothPWSW** | 3; Preserve both PhotoWorks and SOLIDWORKS display states; valid in documents created in SOLIDWORKS 2009 and earlier |
| **swDisplayStateCreation\_PW** | 1; Preserve PhotoWorks material display state only; valid in documents created in SOLIDWORKS 2009 and earlier |
| **swDisplayStateCreation\_SW** | 2; Preserve SOLIDWORKS color display state only; valid in documents created in SOLIDWORKS 2009 and earlier |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)