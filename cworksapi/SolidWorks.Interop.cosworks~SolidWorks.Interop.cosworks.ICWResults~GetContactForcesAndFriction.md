<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetContactForcesAndFriction.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetContactForcesAndFriction Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetContactForcesAndFriction Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NStepNumber*
:   Solution step number at which to calculate the contact forces for non-linear and drop test studies; 1 for static studies

*DispPlane*
:   Plane, axis, or coordinate system relative to which the contact forces are calculated

*ArraySelectedEntities*
:   Array of entities for which to calculate contact forces

*NForceType*
:   Type of contact force as defined in [swsNForceType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNForceType_e.html)

*NUnits*
:   Units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

Gets the specified contact or friction forces for the specified entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetContactForcesAndFriction( _    ByVal NStepNumber As System.Integer, _    ByVal DispPlane As System.Object, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NForceType As System.Integer, _    ByVal NUnits As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim NStepNumber As System.Integer Dim DispPlane As System.Object Dim ArraySelectedEntities As System.Object Dim NForceType As System.Integer Dim NUnits As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetContactForcesAndFriction(NStepNumber, DispPlane, ArraySelectedEntities, NForceType, NUnits, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetContactForcesAndFriction(     System.int NStepNumber,    System.object DispPlane,    System.object ArraySelectedEntities,    System.int NForceType,    System.int NUnits,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetContactForcesAndFriction(  &   System.int NStepNumber, &   System.Object^ DispPlane, &   System.Object^ ArraySelectedEntities, &   System.int NForceType, &   System.int NUnits, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NStepNumber*
:   Solution step number at which to calculate the contact forces for non-linear and drop test studies; 1 for static studies

*DispPlane*
:   Plane, axis, or coordinate system relative to which the contact forces are calculated

*ArraySelectedEntities*
:   Array of entities for which to calculate contact forces

*NForceType*
:   Type of contact force as defined in [swsNForceType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNForceType_e.html)

*NUnits*
:   Units as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*ErrorCode*
:   Error as defined in [swsResultsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultsError_e.html)

#### Return Value

Array of four doubles of the contact forces for all selections in ArraySelectedEntities:

1. Summation of x-components of contact forces- Summation of y-components of contact forces- Summation of z-components of contact forces- Resultant contact force

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetContactForcesAndFriction.

# ![](dotnetimages/collapse.gif)Example

[Get Contact or Friction Forces (VBA)](Get_Normal_Contact_Friction_Force_Example_VB.htm)

[Get Contact or Friction Forces (VB.NET)](Get_Normal_Contact_Friction_Force_Example_VBNET.htm)

[Get Contact or Friction Forces (C#)](Get_Normal_Contact_Friction_Force_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2013 SP0