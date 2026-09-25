<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swPipingPenetrationStatus_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swPipingPenetrationStatus\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swPipingPenetrationStatus\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Piping pentration status.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPipingPenetrationStatus_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPipingPenetrationStatus_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPipingPenetrationStatus_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPipingPenetrationStatus_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swPenetrationFailed** | 1 = Unspecified error |
| **swPenetrationFailedAlreadyPenetrating** | 8 = Pipe is already penetrating |
| **swPenetrationFailedBadFitting** | 7 = Pipe cannot be found or fitting to pierce cannot be found |
| **swPenetrationFailedBadSelection** | 6 = Sketch point cannot be used for penetration |
| **swPenetrationFailedDllNotLoaded** | 3 = Routing not installed |
| **swPenetrationFailedMultiBody** | 9 = Pipe cannot pentrate multibody |
| **swPenetrationFailedNoSelection** | 4 = No sketch point selected |
| **swPenetrationFailedNotRouting** | 5 = Sketch is not a routing sketch |
| **swPenetrationFailedPipeTooWide** | 2 = Pipe too wide to cut other pipe |
| **swPenetrationSucceeded** | 0 = Okay |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)