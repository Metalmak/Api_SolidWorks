<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestResultOptions~GetSensorDetails.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetSensorDetails Method (ICWDropTestResultOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDropTestResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestResultOptions.html) : GetSensorDetails Method (ICWDropTestResultOptions) |

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

Gets the simulation data sensor that is used to report work flow sensitive data.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetSensorDetails( _    ByRef NSensorOption As System.Integer, _    ByRef SSensorName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDropTestResultOptions Dim NSensorOption As System.Integer Dim SSensorName As System.String   instance.GetSensorDetails(NSensorOption, SSensorName) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSensorDetails(     out System.int NSensorOption,    out System.string SSensorName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSensorDetails(  &   [Out] System.int NSensorOption, &   [Out] System.String^ SSensorName ) ``` | |

#### Parameters

*NSensorOption*
:   Sensor option as defined in [swsResultOptionsSensorOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultOptionsSensorOption_e.html)

*SSensorName*
:   Sensor name; valid only if NSensorOption = [swsResultOptionsSensorOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultOptionsSensorOption_e.html).swsResultOptionsSensorOption\_SpecificSensor

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDropTestResultOptions::GetSensorDetails.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDropTestResultOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestResultOptions.html)

[ICWDropTestResultOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestResultOptions_members.html)

[ICWDropTestResultOptions::SetSensorDetails Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestResultOptions~SetSensorDetails.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0