<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~GetMomentComponentValues2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMomentComponentValues2 Method (ICWForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : GetMomentComponentValues2 Method (ICWForce) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*B1*
:   -1 or true if moment about the X direction exists, 0 or false if not (see **Remarks**)

*B2*
:   -1 or true if moment about the Y direction exists, 0 or false if not (see **Remarks**)

*B3*
:   -1 or true if moment about the Z direction exists, 0 or false if not (see **Remarks**)

*D1*
:   Moment about X

*D2*
:   Moment about Y

*D3*
:   Moment about Z

Gets the moment values.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetMomentComponentValues2( _    ByRef B1 As System.Boolean, _    ByRef B2 As System.Boolean, _    ByRef B3 As System.Boolean, _    ByRef D1 As System.Double, _    ByRef D2 As System.Double, _    ByRef D3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim B1 As System.Boolean Dim B2 As System.Boolean Dim B3 As System.Boolean Dim D1 As System.Double Dim D2 As System.Double Dim D3 As System.Double   instance.GetMomentComponentValues2(B1, B2, B3, D1, D2, D3) ``` | |

| C# |  |
| --- | --- |
| ``` void GetMomentComponentValues2(     out System.bool B1,    out System.bool B2,    out System.bool B3,    out System.double D1,    out System.double D2,    out System.double D3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetMomentComponentValues2(  &   [Out] System.bool B1, &   [Out] System.bool B2, &   [Out] System.bool B3, &   [Out] System.double D1, &   [Out] System.double D2, &   [Out] System.double D3 ) ``` | |

#### Parameters

*B1*
:   -1 or true if moment about the X direction exists, 0 or false if not (see **Remarks**)

*B2*
:   -1 or true if moment about the Y direction exists, 0 or false if not (see **Remarks**)

*B3*
:   -1 or true if moment about the Z direction exists, 0 or false if not (see **Remarks**)

*D1*
:   Moment about X

*D2*
:   Moment about Y

*D3*
:   Moment about Z

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::GetMomentComponentValues2.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for models with beam elements and if [ICWForce::ForceType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceType.html) is set to [swsForceType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceType_e.html).swsForceTypeForceOrMoment.

This method returns booleans or integers in out parameters B1, B2, and B3, depending on their prior declarations.

If out parameters B1, B2, and B3 are cast as:

* Booleans, true or false is returned in each out parameter.* Longs or integers, -1 (=true) or 0 (=false) is returned in each out parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04