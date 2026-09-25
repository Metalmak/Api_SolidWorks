<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager~GetFactorOfSafetyConstraint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetFactorOfSafetyConstraint Method (ICWTopologyStudyManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager.html) : GetFactorOfSafetyConstraint Method (ICWTopologyStudyManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SConstraintName*
:   Name of the Factory Of Safety constraint to retrieve

*ErrorCode*
:   Result code as defined in [swsTopologyStudyError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyError_e.html)

Gets the specified Factor Of Safety constraint for this topology study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFactorOfSafetyConstraint( _    ByVal SConstraintName As System.String, _    ByRef ErrorCode As System.Integer _ ) As CWTopologyFactorOfSafetyConstraint ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyStudyManager Dim SConstraintName As System.String Dim ErrorCode As System.Integer Dim value As CWTopologyFactorOfSafetyConstraint   value = instance.GetFactorOfSafetyConstraint(SConstraintName, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWTopologyFactorOfSafetyConstraint GetFactorOfSafetyConstraint(     System.string SConstraintName,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWTopologyFactorOfSafetyConstraint^ GetFactorOfSafetyConstraint(  &   System.String^ SConstraintName, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*SConstraintName*
:   Name of the Factory Of Safety constraint to retrieve

*ErrorCode*
:   Result code as defined in [swsTopologyStudyError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyError_e.html)

#### Return Value

[ICWTopologyFactorOfSafetyConstraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFactorOfSafetyConstraint.html); null if failure

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyStudyManager::GetFactorOfSafetyConstraint.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyStudyManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager.html) example.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyStudyManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager.html)

[ICWTopologyStudyManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyStudyManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0