<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint~SetUnit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetUnit Method (ICWTopologyMassConstraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyMassConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint.html) : SetUnit Method (ICWTopologyMassConstraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NUnit*
:   Units of mass as defined in [swsMassUnits\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMassUnits_e.html) (see **Remarks**)

Sets the units of mass for this topology study mass constraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetUnit( _    ByVal NUnit As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyMassConstraint Dim NUnit As System.Integer Dim value As System.Integer   value = instance.SetUnit(NUnit) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetUnit(     System.int NUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetUnit(  &   System.int NUnit ) ``` | |

#### Parameters

*NUnit*
:   Units of mass as defined in [swsMassUnits\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMassUnits_e.html) (see **Remarks**)

#### Return Value

Result code as defined in [swsTopologyStudy\_MassConstraintErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_MassConstraintErrors_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyMassConstraint::SetUnit.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyMassConstraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWTopologyMassConstraint::SetMassPreference](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint~SetMassPreference.html) sets [swsTopologyStudyMassConstraintOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyMassConstraintOption_e.html).swsTopologyMassConstraintOption\_AbsoluteValue.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyMassConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint.html)

[ICWTopologyMassConstraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint_members.html)

[ICWTopologyMassConstraint::SetValue Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyMassConstraint~SetValue.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0