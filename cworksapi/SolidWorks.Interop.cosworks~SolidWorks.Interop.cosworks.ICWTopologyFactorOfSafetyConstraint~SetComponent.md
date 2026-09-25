<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFactorOfSafetyConstraint~SetComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetComponent Method (ICWTopologyFactorOfSafetyConstraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyFactorOfSafetyConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFactorOfSafetyConstraint.html) : SetComponent Method (ICWTopologyFactorOfSafetyConstraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NComponent*
:   [swsTopologyStudyFactorOfSafetyComponentType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyFactorOfSafetyComponentType_e.html).swsTopologyFactorOfSafetyCompType\_MaxVONMises

Sets the component of this topology study Factor Of Safety constraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetComponent( _    ByVal NComponent As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyFactorOfSafetyConstraint Dim NComponent As System.Integer Dim value As System.Integer   value = instance.SetComponent(NComponent) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetComponent(     System.int NComponent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetComponent(  &   System.int NComponent ) ``` | |

#### Parameters

*NComponent*
:   [swsTopologyStudyFactorOfSafetyComponentType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyFactorOfSafetyComponentType_e.html).swsTopologyFactorOfSafetyCompType\_MaxVONMises

#### Return Value

Result code as defined in [swsTopologyStudy\_FOSConstraintErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_FOSConstraintErrors_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyFactorOfSafetyConstraint::SetComponent.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyFactorOfSafetyConstraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFactorOfSafetyConstraint.html) example.

# ![](dotnetimages/collapse.gif)Remarks

This Factor Of Safety constraint equation:

```
FOS_component comparator value
```

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyFactorOfSafetyConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFactorOfSafetyConstraint.html)

[ICWTopologyFactorOfSafetyConstraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFactorOfSafetyConstraint_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0