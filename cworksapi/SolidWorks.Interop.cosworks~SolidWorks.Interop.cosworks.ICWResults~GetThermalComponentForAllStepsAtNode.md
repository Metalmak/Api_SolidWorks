<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetThermalComponentForAllStepsAtNode.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetThermalComponentForAllStepsAtNode Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetThermalComponentForAllStepsAtNode Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NComponent*
:   Thermal component as defined in [swsThermalComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsThermalComponent_e.html)

*NNodeNum*
:   Node number

*DispPlane*
:   Plane, axis, or coordinate system; valid only if NComponent is set to a directional component; specify nothing if NComponent is a scalar component and not a
    directional component

*NUnits*
:   Temperature unit as defined [swsTemperatureUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTemperatureUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets thermal values at the specified node for all solutions steps.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetThermalComponentForAllStepsAtNode( _    ByVal NComponent As System.Integer, _    ByVal NNodeNum As System.Integer, _    ByVal DispPlane As System.Object, _    ByVal NUnits As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NComponent As System.Integer Dim NNodeNum As System.Integer Dim DispPlane As System.Object Dim NUnits As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetThermalComponentForAllStepsAtNode(NComponent, NNodeNum, DispPlane, NUnits, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetThermalComponentForAllStepsAtNode(     System.int NComponent,    System.int NNodeNum,    System.object DispPlane,    System.int NUnits,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetThermalComponentForAllStepsAtNode(  &   System.int NComponent, &   System.int NNodeNum, &   System.Object^ DispPlane, &   System.int NUnits, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NComponent*
:   Thermal component as defined in [swsThermalComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsThermalComponent_e.html)

*NNodeNum*
:   Node number

*DispPlane*
:   Plane, axis, or coordinate system; valid only if NComponent is set to a directional component; specify nothing if NComponent is a scalar component and not a
    directional component

*NUnits*
:   Temperature unit as defined [swsTemperatureUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsTemperatureUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of thermal results (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetThermalComponentForAllStepsAtNode.

# ![](dotnetimages/collapse.gif)Example

[Get Thermal Values (VBA)](Get_Thermal_Values_at_Points_Example_VB.htm)

[Get Thermal Values (VB.NET)](Get_Thermal_Values_at_Points_Example_VBNET.htm)

[Get Thermal Values (C#)](Get_Thermal_Values_at_Points_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns the following array:

{

*solution\_step\_1*, *time\_1*, *temp\_1,*

*solution\_step\_2*, *time\_2*, *temp\_2,*

*solution\_step\_3*, *time\_3*, *temp\_3,*

     ...,

*solution\_step\_n*, *time\_n*, *temp\_n*

},

where the solution steps are integers, *time\_n* = (*solution\_step\_n* \* 60) seconds, and the temperatures are doubles.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetMinMaxThermal Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxThermal.html)

[ICWResults::GetThermalForEntities Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetThermalForEntities.html)

[ICWResults::GetThermalValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetThermalValues.html)

[ICWResults::GetThermalValuesAtPoints Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetThermalValuesAtPoints.html)

[ICWResults::GetHeatPowerOrEnergy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetHeatPowerOrEnergy.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0