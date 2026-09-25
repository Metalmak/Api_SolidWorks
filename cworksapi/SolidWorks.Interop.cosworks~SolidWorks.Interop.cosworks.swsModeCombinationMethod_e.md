<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsModeCombinationMethod_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsModeCombinationMethod\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsModeCombinationMethod\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Mode combination methods for calculating a peak response in dynamic studies

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsModeCombinationMethod_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsModeCombinationMethod_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsModeCombinationMethod_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsModeCombinationMethod_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsModeCombinationMethod\_AbsSum** | 1 = Absolute Sum; This method calculates the peak response as the sum of the maximum modal responses |
| **swsModeCombinationMethod\_CQC** | 2 = Complete Quadratic Combination (CQC); This method calculates the peak response using cross-modal correlation coefficients, modal damping coefficients, and a double summation equation based on random vibration theories |
| **swsModeCombinationMethod\_NRL** | 3 = Naval Research Laboratory (NRL); This method calculates the peak response as the sum of the absolute value of the response of the mode that exhibits the largest response and the SRSS response of the remaining modes |
| **swsModeCombinationMethod\_SRSS** | 0 = Square Root of the Sum of Squares (SRSS); This method calculates the peak response as the square root of the sum of the maximum modal responses squared |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)