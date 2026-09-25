<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_StressConstraintErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_StressConstraintErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_StressConstraintErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study stress constraint result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_StressConstraintErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_StressConstraintErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_StressConstraintErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_StressConstraintErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoStressErrCode\_ConstraintNotFound** | 10 |
| **swsTopoStressErrCode\_InvalidComparator** | 7 = Only [swsTopologyStudyConstraintComparator\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyConstraintComparator_e.html).swsTopologyConstraintComparator\_IsLessThan is available |
| **swsTopoStressErrCode\_InvalidComponent** | 4 |
| **swsTopoStressErrCode\_InvalidConstraintValuationOption** | 5 |
| **swsTopoStressErrCode\_InvalidConstraintValue** | 2 |
| **swsTopoStressErrCode\_InvalidUnit** | 6 |
| **swsTopoStressErrCode\_LessThanEqualToZeroConstraintValue** | 3 |
| **swsTopoStressErrCode\_LessThanPermittedValue** | 9 = Stress value must be above minimum model stress |
| **swsTopoStressErrCode\_OutOfRangePercentageValue** | 11 = Percentage value for stress must be between 0 and 100 |
| **swsTopoStressErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoStressErrCode\_Success** | 0 |
| **swsTopoStressErrCode\_UnitNotAvailable** | 8 = SetUnit is available only when SetValuationPreference sets NValuationOption = [swsTopologyStudyConstraintValuationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyConstraintValuationOption_e.html).swsTopologyConstraintValuationOption\_AbsValue |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)