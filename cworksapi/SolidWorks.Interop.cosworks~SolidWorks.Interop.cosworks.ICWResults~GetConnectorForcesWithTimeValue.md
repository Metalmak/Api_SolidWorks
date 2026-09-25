<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetConnectorForcesWithTimeValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetConnectorForcesWithTimeValue Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetConnectorForcesWithTimeValue Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DTimeValue*
:   Time at which to get connector values

*SName*
:   Name of a pin, bolt, bearing, spring, spot weld, edge weld, or link connector (see **Remarks**)

*NUnits*
:   Output units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*DAccurateTimeValue*
:   Accurate time

*ErrorCode*
:   Error code as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the component and resultant forces, bending moments, and torques for the specified connector at the specified time.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetConnectorForcesWithTimeValue( _    ByVal DTimeValue As System.Double, _    ByVal SName As System.String, _    ByVal NUnits As System.Integer, _    ByRef DAccurateTimeValue As System.Double, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim DTimeValue As System.Double Dim SName As System.String Dim NUnits As System.Integer Dim DAccurateTimeValue As System.Double Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetConnectorForcesWithTimeValue(DTimeValue, SName, NUnits, DAccurateTimeValue, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetConnectorForcesWithTimeValue(     System.double DTimeValue,    System.string SName,    System.int NUnits,    out System.double DAccurateTimeValue,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetConnectorForcesWithTimeValue(  &   System.double DTimeValue, &   System.String^ SName, &   System.int NUnits, &   [Out] System.double DAccurateTimeValue, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*DTimeValue*
:   Time at which to get connector values

*SName*
:   Name of a pin, bolt, bearing, spring, spot weld, edge weld, or link connector (see **Remarks**)

*NUnits*
:   Output units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*DAccurateTimeValue*
:   Accurate time

*ErrorCode*
:   Error code as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of 16 doubles:

* x-component of the shear force* y-component of the shear force* z-component of the shear force* Resultant shear force* x-component of the axial force* y-component of the axial force* z-component of the axial force* Resultant axial force* x-component of the bending moment* y-component of the bending moment* z-component of the bending moment* Resultant bending moment* x-component of the torque* y-component of the torque* z-component of the torque* Resultant torque

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetConnectorForcesWithTimeValue.

# ![](dotnetimages/collapse.gif)Example

[Get Connector Forces, Moments, and Torques at a Time (VBA)](Get_Connector_Forces_at_a_Time_Example_VB.htm)

[Get Connector Forces, Moments, and Torques at a Time (VB.NET)](Get_Connector_Forces_at_a_Time_Example_VBNET.htm)

[Get Connector Forces, Moments, and Torques at a Time (C#)](Get_Connector_Forces_at_a_Time_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

For spot welds, specify SName with the spot weld point (e.g., "Spot Welds-1/Point1").

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetConnectorForces2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetConnectorForces2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0