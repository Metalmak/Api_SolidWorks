<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_DisplacementConstraintErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsTopologyStudy\_DisplacementConstraintErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsTopologyStudy\_DisplacementConstraintErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Topology study displacement constraint result codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsTopologyStudy_DisplacementConstraintErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsTopologyStudy_DisplacementConstraintErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsTopologyStudy_DisplacementConstraintErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsTopologyStudy_DisplacementConstraintErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsTopoDispErrCode\_CannotSetVertex** | 10 = SetVertex is available only when LocationOption = [swsTopologyStudyDisplacementConstraintLocationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementConstraintLocationOption_e.html).swsTopologyDisplacementConstraintLocationOption\_UserDefine |
| **swsTopoDispErrCode\_ConstraintNotFound** | 17 = Constraint does not exist |
| **swsTopoDispErrCode\_CoordinateSysInvalidOption** | 14 = Option must be in [swsTopologyStudyDisplacementCoordinateSysOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementCoordinateSysOption_e.html) |
| **swsTopoDispErrCode\_CoordinateSysInvalidSelection** | 15 = Wrong coordinate system dispatch was passed |
| **swsTopoDispErrCode\_CoordinateSysNAError** | 13 = SetCoordinateSystem is available only when SetCoordinateSystemPreference sets NCSPreference = [swsTopologyStudyDisplacementCoordinateSysOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementCoordinateSysOption_e.html).swsTopologyDisplacementCoordinateSysOption\_UserDefine |
| **swsTopoDispErrCode\_CoordinateSysNotSelected** | 16 = Coordinate system has not been set |
| **swsTopoDispErrCode\_InvalidArray** | 18 = Invalid input array |
| **swsTopoDispErrCode\_InvalidComparator** | 7 = Input comparator must be in [swsTopologyStudyConstraintComparator\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyConstraintComparator_e.html) |
| **swsTopoDispErrCode\_InvalidComponent** | 4 = Component type must be in [swsTopologyStudyDisplacementComponentType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementComponentType_e.html) |
| **swsTopoDispErrCode\_InvalidConstraintValuationOption** | 5 = Valuation option must be in [swsTopologyStudyConstraintValuationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyConstraintValuationOption_e.html) |
| **swsTopoDispErrCode\_InvalidConstraintValue** | 2 = Input value contains invalid characters |
| **swsTopoDispErrCode\_InvalidLocationOption** | 11 = Location option must be in [swsTopologyDisplacementConstraintLocationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyDisplacementConstraintLocationOption_e.html) |
| **swsTopoDispErrCode\_InvalidSelectionForVertex** | 9 = Wrong vertex dispatch has been passed |
| **swsTopoDispErrCode\_InvalidUnit** | 6 = Input unit must be in [swsLinearUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLinearUnit_e.html) |
| **swsTopoDispErrCode\_InvalidVertexCount** | 12 = You cannot define this displacement constraint when SetLocationPreference sets NLocationPreference = swsTopologyStudyDisplacementConstraintLocationOption\_e.swsTopologyDisplacementConstraintLocationOption\_UserDefine and vertex count != 1 |
| **swsTopoDispErrCode\_LessThanEqualToZeroConstraintValue** | 3 = Less than or equal to zero value is invalid |
| **swsTopoDispErrCode\_SetOperationNotSupported** | 1 = BeginEdit must be called before setting values |
| **swsTopoDispErrCode\_Success** | 0 |
| **swsTopoDispErrCode\_UnitNotAvailable** | 8 = SetUnit is available only when SetValuationPreference sets NValuationOption = [swsTopologyStudyConstraintValuationOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyConstraintValuationOption_e.html).swsTopologyConstraintValuationOption\_AbsValue |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)