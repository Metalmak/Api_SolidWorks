<!-- source: dsgnchkapi/SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.dsgnchkError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Design Checker API Help | Send comments on this topic. |
| dsgnchkError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.dsgnchk Namespace](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk_namespace.html) : dsgnchkError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

SOLIDWORKS Design Checker status

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum dsgnchkError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As dsgnchkError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum dsgnchkError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class dsgnchkError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **dsgnchkAllStandardFilesInvalid** | 6 = All standard files invalid |
| **dsgnchkCouldNotCreateReportDirectory** | 2 = Error creating report folder |
| **dsgnchkDesignCheckerAlreadyRunning** | 7 = SOLIDWORKS Design Checker already running; you must close the running Design Checker process before running a new SOLIDWORKS Design Checker process |
| **dsgnchkInvalidCallToAPI** | 8 = Invalid call to SOLIDWORKS Design Checker API |
| **dsgnchkInvalidReportName** | 5 = Invalid report name |
| **dsgnchkNoActivedocument** | 3 = No active document |
| **dsgnchkNOErr** | 0 = No errors |
| **dsgnchkReportAlreadyExists** | 1 = Report already exists |
| **dsgnchkStandardFileDoesNotExist** | 4 = Requirements file does not exist |
| **dsgnchkUnknownErr** | -1 = Unknown errors |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.dsgnchk Namespace](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk_namespace.html)