<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFrequencyConstraint~SetFrequencyData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetFrequencyData Method (ICWTopologyFrequencyConstraint) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTopologyFrequencyConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFrequencyConstraint.html) : SetFrequencyData Method (ICWTopologyFrequencyConstraint) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarModeShapes*
:   Array of mode shape numbers (see **Remarks**)

*VarComparators*
:   Array of [swsTopologyStudyConstraintComparator\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyConstraintComparator_e.html) (see **Remarks**)

*VarFrequencyValues*
:   Array of frequency values (see **Remarks**)

Sets the equations for this topology study frequency constraint.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetFrequencyData( _    ByVal VarModeShapes As System.Object, _    ByVal VarComparators As System.Object, _    ByVal VarFrequencyValues As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTopologyFrequencyConstraint Dim VarModeShapes As System.Object Dim VarComparators As System.Object Dim VarFrequencyValues As System.Object Dim value As System.Integer   value = instance.SetFrequencyData(VarModeShapes, VarComparators, VarFrequencyValues) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetFrequencyData(     System.object VarModeShapes,    System.object VarComparators,    System.object VarFrequencyValues ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetFrequencyData(  &   System.Object^ VarModeShapes, &   System.Object^ VarComparators, &   System.Object^ VarFrequencyValues ) ``` | |

#### Parameters

*VarModeShapes*
:   Array of mode shape numbers (see **Remarks**)

*VarComparators*
:   Array of [swsTopologyStudyConstraintComparator\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudyConstraintComparator_e.html) (see **Remarks**)

*VarFrequencyValues*
:   Array of frequency values (see **Remarks**)

#### Return Value

Result code as defined in [swsTopologyStudy\_FrequencyConstraintErrors\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTopologyStudy_FrequencyConstraintErrors_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTopologyFrequencyConstraint::SetFrequencyData.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTopologyFrequencyConstraint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFrequencyConstraint.html) example.

# ![](dotnetimages/collapse.gif)Remarks

The arrays of VarModeShapes, VarComparators, and VarFrequencyValues map one-to-one and onto. Together they define *n* frequency constraint equations as follows:

```
for i = 0 to n-1
```

```
  VarModeShapes[i] VarComparators[i] VarFrequencyValues[i]
```

```
next  i
```

The VarModeShapes array must be in mode shape ascending order, and the VarFrequencyValues array must be in frequency ascending order.

If the VarComparators array contains swsTopologyStudyConstraintComparator\_e.swsTopologyConstraintComparator\_IsInBetween, then the corresponding value in VarFrequencyValues must be specified with a range of values, e.g., "200-400".

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTopologyFrequencyConstraint Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFrequencyConstraint.html)

[ICWTopologyFrequencyConstraint Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFrequencyConstraint_members.html)

[ICWTopologyFrequencyConstraint::ClearFrequencyData Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTopologyFrequencyConstraint~ClearFrequencyData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2019 SP0