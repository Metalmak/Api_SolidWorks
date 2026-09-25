<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_FrequencyConstraintErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_FrequencyConstraintErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_FrequencyConstraintErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study frequency constraint result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_FrequencyConstraintErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_FrequencyConstraintErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_FrequencyConstraintErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_FrequencyConstraintErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoFreqErrCode\_ComparatorDataIsNotSet** | 12 |
| **swsTopoFreqErrCode\_ConstraintNotFound** | 15 |
| **swsTopoFreqErrCode\_EnterRangeOfValues** | 6 = If SetFrequencyData sets an element of the VarComparators array with [swsTopologyStudyConstraintComparator\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyConstraintComparator_e.html).swsTopologyConstraintComparator\_IsInBetween, then the corresponding value in the VarFrequencyValues array must be specified with a range of values, e.g., "200-400".  In-between comparator requires a range of values (e.g., 200-400) |
| **swsTopoFreqErrCode\_FreqValuesDataIsNotSet** | 13 |
| **swsTopoFreqErrCode\_HMSFreqLessThanLMSFreq** | 4 = You must set the arrays in SetFrequencyData such that higher mode shapes have frequency values greater than those of lower mode shapes, i.e., VarModeShapes and VarFrequencyValues arrays must both be in increasing order |
| **swsTopoFreqErrCode\_InvalidArray** | 14 |
| **swsTopoFreqErrCode\_InvalidComparatorData** | 9 |
| **swsTopoFreqErrCode\_InvalidConstraintValue** | 2 |
| **swsTopoFreqErrCode\_InvalidFreqValuesData** | 10 |
| **swsTopoFreqErrCode\_InvalidModeShapeData** | 8 |
| **swsTopoFreqErrCode\_LessThanEqualToZeroConstraintValue** | 3 |
| **swsTopoFreqErrCode\_ModeShapeDataIsNotSet** | 11 |
| **swsTopoFreqErrCode\_ModeShapesNotInAscendingOrder** | 5 |
| **swsTopoFreqErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoFreqErrCode\_Success** | 0 |
| **swsTopoFreqErrCode\_UnequalSizedArrays** | 7 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)