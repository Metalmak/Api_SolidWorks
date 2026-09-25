<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint~SetMassPreference.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMassPreference Method (ICWTopologyMassConstraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyMassConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint.html) : SetMassPreference Method (ICWTopologyMassConstraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NPreference*
:   Reduce-mass-by preference as defined in [swsTopologyStudyMassConstraintOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyMassConstraintOption_e.html)

Sets the reduce-mass-by preference for this topology study mass constraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetMassPreference( _    ByVal NPreference As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyMassConstraint Dim NPreference As System.Integer Dim value As System.Integer   value = instance.SetMassPreference(NPreference) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetMassPreference(     System.int NPreference ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetMassPreference(  &   System.int NPreference ) ``` | |

#### Parameters

*NPreference*
:   Reduce-mass-by preference as defined in [swsTopologyStudyMassConstraintOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyMassConstraintOption_e.html)

#### Return Value

Result code as defined in [swsTopologyStudy\_MassConstraintErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_MassConstraintErrors_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyMassConstraint::SetMassPreference.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyMassConstraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint.html) example.

# ![](dotnetimages/collapse.gif)Remarks

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyMassConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint.html)

[ICWTopologyMassConstraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0