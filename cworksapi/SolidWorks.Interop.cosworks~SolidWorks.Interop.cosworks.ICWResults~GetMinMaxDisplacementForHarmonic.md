<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxDisplacementForHarmonic.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMinMaxDisplacementForHarmonic Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetMinMaxDisplacementForHarmonic Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NComponent*
:   Displacement component as defined in [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html)

*NStepNum*
:   Solution step number (use 1 for static)

*DispPlane*
:   Plane, axis, or coordinate system; valid only if NComponent is set to a directional component; specify nothing if reference geometry does not exist

*NUnits*
:   Linear units for displacement translation as defined in [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the algebraic minimum and maximum displacement for the specified component and solution step of this harmonic study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMinMaxDisplacementForHarmonic( _    ByVal NComponent As System.Integer, _    ByVal NStepNum As System.Integer, _    ByVal DispPlane As System.Object, _    ByVal NUnits As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NComponent As System.Integer Dim NStepNum As System.Integer Dim DispPlane As System.Object Dim NUnits As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetMinMaxDisplacementForHarmonic(NComponent, NStepNum, DispPlane, NUnits, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMinMaxDisplacementForHarmonic(     System.int NComponent,    System.int NStepNum,    System.object DispPlane,    System.int NUnits,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMinMaxDisplacementForHarmonic(  &   System.int NComponent, &   System.int NStepNum, &   System.Object^ DispPlane, &   System.int NUnits, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NComponent*
:   Displacement component as defined in [swsDisplacementComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsDisplacementComponent_e.html)

*NStepNum*
:   Solution step number (use 1 for static)

*DispPlane*
:   Plane, axis, or coordinate system; valid only if NComponent is set to a directional component; specify nothing if reference geometry does not exist

*NUnits*
:   Linear units for displacement translation as defined in [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetMinMaxDisplacementForHarmonic.

# ![](dotnetimages/collapse.gif)Remarks

This method returns the following array:

{*node\_with\_minimum\_displacement*, *minimum\_displacement*, *node\_with\_maximum\_displacement*, *maximum\_displacement*},

where the nodes are integer indexes, and the displacements are in scientific notation.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetMinMaxDisplacement Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxDisplacement.html)

[ICWResults::GetMinMaxDisplacementRMS Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxDisplacementRMS.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP1.0