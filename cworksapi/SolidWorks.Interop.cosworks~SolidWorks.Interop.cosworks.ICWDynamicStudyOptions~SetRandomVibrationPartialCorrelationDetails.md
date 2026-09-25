<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationPartialCorrelationDetails.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetRandomVibrationPartialCorrelationDetails Method (ICWDynamicStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html) : SetRandomVibrationPartialCorrelationDetails Method (ICWDynamicStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NUnits*
:   Units as defined [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*DInRadius*
:   Inside radius

*DOutRadius*
:   Outside radius

Obsolete. Superseded by [ICWDynamicStudyOptions::SetRandomVibrationPartialCorrelationDetails2.](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDynamicStudyOptions~SetRandomVibrationPartialCorrelationDetails2.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetRandomVibrationPartialCorrelationDetails( _    ByVal NUnits As System.Integer, _    ByVal DInRadius As System.Double, _    ByVal DOutRadius As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDynamicStudyOptions Dim NUnits As System.Integer Dim DInRadius As System.Double Dim DOutRadius As System.Double   instance.SetRandomVibrationPartialCorrelationDetails(NUnits, DInRadius, DOutRadius) ``` | |

| C# |  |
| --- | --- |
| ``` void SetRandomVibrationPartialCorrelationDetails(     System.int NUnits,    System.double DInRadius,    System.double DOutRadius ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetRandomVibrationPartialCorrelationDetails(  &   System.int NUnits, &   System.double DInRadius, &   System.double DOutRadius ) ``` | |

#### Parameters

*NUnits*
:   Units as defined [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*DInRadius*
:   Inside radius

*DOutRadius*
:   Outside radius

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDynamicStudyOptions::SetRandomVibrationPartialCorrelationDetails.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDynamicStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions.html)

[ICWDynamicStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDynamicStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0