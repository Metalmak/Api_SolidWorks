<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions~SetSensorDetailsForGraphsAndPlots.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetSensorDetailsForGraphsAndPlots Method (ICWStudyResultOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html) : SetSensorDetailsForGraphsAndPlots Method (ICWStudyResultOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NSensorOption*
:   Sensor option as defined in [swsResultOptionsSensorOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultOptionsSensorOption_e.html)

*SSensorName*
:   Sensor name; valid only if NSensorOption = [swsResultOptionsSensorOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultOptionsSensorOption_e.html).swsResultOptionsSensorOption\_SpecificSensor

Sets how plot data for response graphs is saved.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetSensorDetailsForGraphsAndPlots( _    ByVal NSensorOption As System.Integer, _    ByVal SSensorName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudyResultOptions Dim NSensorOption As System.Integer Dim SSensorName As System.String   instance.SetSensorDetailsForGraphsAndPlots(NSensorOption, SSensorName) ``` | |

| C# |  |
| --- | --- |
| ``` void SetSensorDetailsForGraphsAndPlots(     System.int NSensorOption,    System.string SSensorName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetSensorDetailsForGraphsAndPlots(  &   System.int NSensorOption, &   System.String^ SSensorName ) ``` | |

#### Parameters

*NSensorOption*
:   Sensor option as defined in [swsResultOptionsSensorOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultOptionsSensorOption_e.html)

*SSensorName*
:   Sensor name; valid only if NSensorOption = [swsResultOptionsSensorOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultOptionsSensorOption_e.html).swsResultOptionsSensorOption\_SpecificSensor

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudyResultOptions::SetSensorDetailsForGraphsAndPlots.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWStudyResultOptions::SaveResultsForSolutionStepsOption](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWStudyResultOptions~SaveResultsForSolutionStepsOption.html) = swsSaveResultsOption\_e.swsSaveResultsOption\_ForSpecifiedSolutionSteps.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudyResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions.html)

[ICWStudyResultOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudyResultOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0