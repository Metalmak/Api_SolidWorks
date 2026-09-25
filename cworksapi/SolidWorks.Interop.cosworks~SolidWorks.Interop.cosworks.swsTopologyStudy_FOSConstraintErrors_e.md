<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_FOSConstraintErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_FOSConstraintErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_FOSConstraintErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study Factor of Safety constraint result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_FOSConstraintErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_FOSConstraintErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_FOSConstraintErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_FOSConstraintErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoFOSErrCode\_ConstraintNotFound** | 7 |
| **swsTopoFOSErrCode\_InvalidComparator** | 6 |
| **swsTopoFOSErrCode\_InvalidComponent** | 4 |
| **swsTopoFOSErrCode\_InvalidConstraintValue** | 2 |
| **swsTopoFOSErrCode\_LessThanEqualToZeroConstraintValue** | 3 |
| **swsTopoFOSErrCode\_MaterialWithInvalidYieldStrength** | 8 = Cannot define FOS for model with material which has invalid yield strength; apply material with valid yield strength |
| **swsTopoFOSErrCode\_OutOfRangeValue** | 5 = Value must be between 1.0 and 10000.0, inclusive |
| **swsTopoFOSErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoFOSErrCode\_Success** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)