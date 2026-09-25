<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~SetMomentComponentValues2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMomentComponentValues2 Method (ICWForce) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html) : SetMomentComponentValues2 Method (ICWForce) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*B1*
:   -1 or true to set moment along plane dir 1, 0 or false to not (see **Remarks**)

*B2*
:   -1 or true to set moment along plane dir 2, 0 or false to not (see **Remarks**)

*B3*
:   -1 or true to set moment along the normal to plane, 0 or false to not (see **Remarks**)

*D1*
:   Moment about plane dir 1

*D2*
:   Moment about plane dir 2

*D3*
:   Moment about normal to plane

Sets the moment values.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMomentComponentValues2( _    ByVal B1 As System.Boolean, _    ByVal B2 As System.Boolean, _    ByVal B3 As System.Boolean, _    ByVal D1 As System.Double, _    ByVal D2 As System.Double, _    ByVal D3 As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWForce Dim B1 As System.Boolean Dim B2 As System.Boolean Dim B3 As System.Boolean Dim D1 As System.Double Dim D2 As System.Double Dim D3 As System.Double   instance.SetMomentComponentValues2(B1, B2, B3, D1, D2, D3) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMomentComponentValues2(     System.bool B1,    System.bool B2,    System.bool B3,    System.double D1,    System.double D2,    System.double D3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMomentComponentValues2(  &   System.bool B1, &   System.bool B2, &   System.bool B3, &   System.double D1, &   System.double D2, &   System.double D3 ) ``` | |

#### Parameters

*B1*
:   -1 or true to set moment along plane dir 1, 0 or false to not (see **Remarks**)

*B2*
:   -1 or true to set moment along plane dir 2, 0 or false to not (see **Remarks**)

*B3*
:   -1 or true to set moment along the normal to plane, 0 or false to not (see **Remarks**)

*D1*
:   Moment about plane dir 1

*D2*
:   Moment about plane dir 2

*D3*
:   Moment about normal to plane

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWForce::SetMomentComponentValues2.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for models with beam elements and if [ICWForce::ForceType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce~ForceType.html) is set to [swsForceType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsForceType_e.html).swsForceTypeForceOrMoment.

Specify booleans or integers in parameters B1, B2, and B3: true = -1 and false = 0.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWForce Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce.html)

[ICWForce Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWForce_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04