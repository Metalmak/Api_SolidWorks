<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_MassConstraintErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_MassConstraintErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_MassConstraintErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study mass constraint result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_MassConstraintErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_MassConstraintErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_MassConstraintErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_MassConstraintErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoMassErrCode\_ConstraintNotFound** | 8 |
| **swsTopoMassErrCode\_GreaterThan100PercentApplied** | 4 = You must specify a percentage of mass to remove that is less than or equal to 100 |
| **swsTopoMassErrCode\_GreaterThanTotalMassOfModel** | 5 = You must specify a quantity of mass to remove that is less than or equal to the total mass of the model |
| **swsTopoMassErrCode\_InvalidConstraintValue** | 2 |
| **swsTopoMassErrCode\_InvalidPreferenceOption** | 7 |
| **swsTopoMassErrCode\_InvalidUnit** | 6 |
| **swsTopoMassErrCode\_LessThanEqualToZeroConstraintValue** | 3 |
| **swsTopoMassErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoMassErrCode\_Success** | 0 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)