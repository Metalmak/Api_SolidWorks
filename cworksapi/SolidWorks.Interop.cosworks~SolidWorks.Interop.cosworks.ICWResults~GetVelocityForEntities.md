<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetVelocityForEntities.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetVelocityForEntities Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetVelocityForEntities Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NComponent*
:   Velocity component as defined in [swsVelocityComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsVelocityComponent_e.html)

*NStepNumber*
:   Solution step number (use 1 for steady state)

*DispPlane*
:   Plane, axis, or coordinate system; valid only if NComponent is set to a directional component; specify nothing if NComponent is not a directional component

*ArraySelectedEntities*
:   Array of geometric entities

*NUnits*
:   Units of velocity as defined in [swsVelocityUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsVelocityUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the specified velocity component for the specified entities and at the specified solution step.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetVelocityForEntities( _    ByVal NComponent As System.Integer, _    ByVal NStepNumber As System.Integer, _    ByVal DispPlane As System.Object, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NUnits As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NComponent As System.Integer Dim NStepNumber As System.Integer Dim DispPlane As System.Object Dim ArraySelectedEntities As System.Object Dim NUnits As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetVelocityForEntities(NComponent, NStepNumber, DispPlane, ArraySelectedEntities, NUnits, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetVelocityForEntities(     System.int NComponent,    System.int NStepNumber,    System.object DispPlane,    System.object ArraySelectedEntities,    System.int NUnits,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetVelocityForEntities(  &   System.int NComponent, &   System.int NStepNumber, &   System.Object^ DispPlane, &   System.Object^ ArraySelectedEntities, &   System.int NUnits, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NComponent*
:   Velocity component as defined in [swsVelocityComponent\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsVelocityComponent_e.html)

*NStepNumber*
:   Solution step number (use 1 for steady state)

*DispPlane*
:   Plane, axis, or coordinate system; valid only if NComponent is set to a directional component; specify nothing if NComponent is not a directional component

*ArraySelectedEntities*
:   Array of geometric entities

*NUnits*
:   Units of velocity as defined in [swsVelocityUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsVelocityUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetVelocityForEntities.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0