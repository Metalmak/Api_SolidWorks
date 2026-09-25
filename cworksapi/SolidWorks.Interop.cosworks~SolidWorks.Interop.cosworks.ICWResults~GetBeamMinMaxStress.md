<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetBeamMinMaxStress.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetBeamMinMaxStress Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetBeamMinMaxStress Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NComponent*
:   Beam stresses as defined in [swsBeamStressComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsBeamStressComponent_e.html)

*NStepNumber*
:   Solution step number (use 1 for static)

*NUnits*
:   Stress units as defined in [swsStrengthUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrengthUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the minimum and maximum elemental stresses for beams at the specified solution step.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBeamMinMaxStress( _    ByVal NComponent As System.Integer, _    ByVal NStepNumber As System.Integer, _    ByVal NUnits As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NComponent As System.Integer Dim NStepNumber As System.Integer Dim NUnits As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetBeamMinMaxStress(NComponent, NStepNumber, NUnits, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetBeamMinMaxStress(     System.int NComponent,    System.int NStepNumber,    System.int NUnits,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetBeamMinMaxStress(  &   System.int NComponent, &   System.int NStepNumber, &   System.int NUnits, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NComponent*
:   Beam stresses as defined in [swsBeamStressComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsBeamStressComponent_e.html)

*NStepNumber*
:   Solution step number (use 1 for static)

*NUnits*
:   Stress units as defined in [swsStrengthUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStrengthUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of stress results for the beams

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetBeamMinMaxStress.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetBeamForcesForEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetBeamForcesForEntities.html)

[ICWResults::GetBeamRadius Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetBeamRadius.html)

[ICWResults::GetBeamStressForEntities Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetBeamStressForEntities.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP1