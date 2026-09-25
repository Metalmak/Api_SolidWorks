<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetForceComponentValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetForceComponentValues Method (ICWForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : SetForceComponentValues Method (ICWForce) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*B1*
:   1 if force in the X direction exists, 0 if not

*B2*
:   1 if force in the Y direction exists, 0 if not

*B3*
:   1 if force in the Z direction exists, 0 if not

*D1*
:   Force in the X direction

*D2*
:   Force in the Y direction

*D3*
:   Force in the Z direction

Obsolete. Superseded by [ICWForce::SetForceComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetForceComponentValues2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetForceComponentValues( _    ByVal B1 As System.Integer, _    ByVal B2 As System.Integer, _    ByVal B3 As System.Integer, _    ByVal D1 As System.Double, _    ByVal D2 As System.Double, _    ByVal D3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim B1 As System.Integer Dim B2 As System.Integer Dim B3 As System.Integer Dim D1 As System.Double Dim D2 As System.Double Dim D3 As System.Double   instance.SetForceComponentValues(B1, B2, B3, D1, D2, D3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetForceComponentValues(     System.int B1,    System.int B2,    System.int B3,    System.double D1,    System.double D2,    System.double D3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetForceComponentValues(  &   System.int B1, &   System.int B2, &   System.int B3, &   System.double D1, &   System.double D2, &   System.double D3 ) ``` | |

#### Parameters

*B1*
:   1 if force in the X direction exists, 0 if not

*B2*
:   1 if force in the Y direction exists, 0 if not

*B3*
:   1 if force in the Z direction exists, 0 if not

*D1*
:   Force in the X direction

*D2*
:   Force in the Y direction

*D3*
:   Force in the Z direction

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::SetForceComponentValues.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid if [ICWForce::ForceType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceType.html) is set to [swsForceType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceType_e.html).swsForceTypeForceOrMoment.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

[ICWForce::GetForceComponentValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetForceComponentValues.html)

[ICWForce::ForceType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceType.html)

[ICWForce::SetReferenceGeometry Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetReferenceGeometry.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0