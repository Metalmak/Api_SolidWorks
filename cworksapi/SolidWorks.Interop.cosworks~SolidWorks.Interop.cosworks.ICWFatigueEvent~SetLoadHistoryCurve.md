<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent~SetLoadHistoryCurve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetLoadHistoryCurve Method (ICWFatigueEvent) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWFatigueEvent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html) : SetLoadHistoryCurve Method (ICWFatigueEvent) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VarLHCurveXData*
:   Array of times; valid only if NType = [swsFatigueLoadHistoryCurveType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueLoadHistoryCurveType_e.html).swsFatigueLoadHistoryCurveType\_TimeAndAmplitude

*VarLHCurveYData*
:   Array of amplitudes

*NType*
:   Type of curve as defined in [swsFatigueLoadHistoryCurveType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueLoadHistoryCurveType_e.html)

*DSamplingRate*
:   Sampling rate in seconds; valid only if NType = [swsFatigueLoadHistoryCurveType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueLoadHistoryCurveType_e.html).swsFatigueLoadHistoryCurveType\_SamplingRateAndAmplitude

Sets the load history curve data for this variable amplitude fatigue event.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetLoadHistoryCurve( _    ByVal VarLHCurveXData As System.Object, _    ByVal VarLHCurveYData As System.Object, _    ByVal NType As System.Integer, _    ByVal DSamplingRate As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWFatigueEvent Dim VarLHCurveXData As System.Object Dim VarLHCurveYData As System.Object Dim NType As System.Integer Dim DSamplingRate As System.Double Dim value As System.Integer   value = instance.SetLoadHistoryCurve(VarLHCurveXData, VarLHCurveYData, NType, DSamplingRate) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetLoadHistoryCurve(     System.object VarLHCurveXData,    System.object VarLHCurveYData,    System.int NType,    System.double DSamplingRate ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetLoadHistoryCurve(  &   System.Object^ VarLHCurveXData, &   System.Object^ VarLHCurveYData, &   System.int NType, &   System.double DSamplingRate ) ``` | |

#### Parameters

*VarLHCurveXData*
:   Array of times; valid only if NType = [swsFatigueLoadHistoryCurveType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueLoadHistoryCurveType_e.html).swsFatigueLoadHistoryCurveType\_TimeAndAmplitude

*VarLHCurveYData*
:   Array of amplitudes

*NType*
:   Type of curve as defined in [swsFatigueLoadHistoryCurveType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueLoadHistoryCurveType_e.html)

*DSamplingRate*
:   Sampling rate in seconds; valid only if NType = [swsFatigueLoadHistoryCurveType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueLoadHistoryCurveType_e.html).swsFatigueLoadHistoryCurveType\_SamplingRateAndAmplitude

#### Return Value

Error code as defined in [swsFatigueEventEndEditError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueEventEndEditError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWFatigueEvent::SetLoadHistoryCurve.

# ![](dotnetimages/collapse.gif)Example

See the [ICWFatigueEvent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWFatigueEvent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent.html)

[ICWFatigueEvent Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent_members.html)

[ICWFatigueEvent::GetLoadHistoryCurve Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFatigueEvent~GetLoadHistoryCurve.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0