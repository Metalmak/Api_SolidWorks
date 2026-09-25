<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCreateExplodeStepError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCreateExplodeStepError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCreateExplodeStepError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Return codes when creating an explode step.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCreateExplodeStepError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCreateExplodeStepError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCreateExplodeStepError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCreateExplodeStepError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCreateExplodeStepError\_EditingComponentInContext** | 6 = A component being edited in context is blocking explode step creation. |
| **swCreateExplodeStepError\_Generic** | 1 = Explode step creation failed. |
| **swCreateExplodeStepError\_InvalidRadialAxis** | 4 = A radial explode step is not allowed using the selected components. |
| **swCreateExplodeStepError\_NoComponents** | 3 = Components to move must be selected. |
| **swCreateExplodeStepError\_NoExplodeView** | 2 = An explode view must be active in the current configuration to create an explode step. |
| **swCreateExplodeStepError\_OpenExplodePMP** | 5 = The open Explode PropertyManager is blocking step creation. |
| **swCreateExplodeStepError\_Successful** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)