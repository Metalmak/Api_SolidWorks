<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetMomentComponentValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMomentComponentValues Method (ICWForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : GetMomentComponentValues Method (ICWForce) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*B1*
:   1 if moment about the X direction exists, 0 if not

*B2*
:   1 if moment about the Y direction exists, 0 if not

*B3*
:   1 if moment about the Z direction exists, 0 if not

*D1*
:   Moment about X

*D2*
:   Moment about Y

*D3*
:   Moment about Z

Obsolete. Superseded by [ICWForce::GetMomentComponentValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetMomentComponentValues2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetMomentComponentValues( _    ByRef B1 As System.Integer, _    ByRef B2 As System.Integer, _    ByRef B3 As System.Integer, _    ByRef D1 As System.Double, _    ByRef D2 As System.Double, _    ByRef D3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim B1 As System.Integer Dim B2 As System.Integer Dim B3 As System.Integer Dim D1 As System.Double Dim D2 As System.Double Dim D3 As System.Double   instance.GetMomentComponentValues(B1, B2, B3, D1, D2, D3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetMomentComponentValues(     out System.int B1,    out System.int B2,    out System.int B3,    out System.double D1,    out System.double D2,    out System.double D3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetMomentComponentValues(  &   [Out] System.int B1, &   [Out] System.int B2, &   [Out] System.int B3, &   [Out] System.double D1, &   [Out] System.double D2, &   [Out] System.double D3 ) ``` | |

#### Parameters

*B1*
:   1 if moment about the X direction exists, 0 if not

*B2*
:   1 if moment about the Y direction exists, 0 if not

*B3*
:   1 if moment about the Z direction exists, 0 if not

*D1*
:   Moment about X

*D2*
:   Moment about Y

*D3*
:   Moment about Z

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::GetMomentComponentValues.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for models with beam elements and if [ICWForce::ForceType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceType.html) is set to [swsForceType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceType_e.html).swsForceTypeForceOrMoment.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

[ICWForce::SetMomentComponentValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetMomentComponentValues.html)

[ICWForce::ForceType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceType.html)

[ICWForce::SetReferenceGeometry Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetReferenceGeometry.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0