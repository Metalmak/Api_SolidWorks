<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_SymmetryControlErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_SymmetryControlErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_SymmetryControlErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study symmetry manufacturing control result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_SymmetryControlErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_SymmetryControlErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_SymmetryControlErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_SymmetryControlErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoSCErrCode\_IncorrectPlaneSelectionsForGivenSymmetryType** | 4 = For [swsTopologySymmetryControlOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologySymmetryControlOption_e.html):   * swsTopologySymmetryControlType\_HalfSymmetry, a single plane can be selected* swsTopologySymmetryControlType\_QuarterSymmetry, two planes can be selected* swsTopologySymmetryControlType\_OneEighthSymmetry, three planes can be selected |
| **swsTopoSCErrCode\_InvalidEntitySelectedAsPlane** | 2 |
| **swsTopoSCErrCode\_InvalidTypeSelected** | 3 |
| **swsTopoSCErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoSCErrCode\_SetSymmetryTypeBeforeSelectingPlane** | 5 |
| **swsTopoSCErrCode\_Success** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)