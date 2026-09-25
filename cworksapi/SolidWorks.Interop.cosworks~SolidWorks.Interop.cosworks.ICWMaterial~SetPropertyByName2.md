<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetPropertyByName2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetPropertyByName2 Method (ICWMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : SetPropertyByName2 Method (ICWMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SName*
:   Property name; for example, 'EX' for Elastic modulus, 'NUXY' for Poisson's ratio, etc.

*DValue*
:   Value of material property

*BValue*
:   -1 or true if temperature dependent, 0 or false if not (see **Remarks**)

Sets the value of the specified material property.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetPropertyByName2( _    ByVal SName As System.String, _    ByVal DValue As System.Double, _    ByVal BValue As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim SName As System.String Dim DValue As System.Double Dim BValue As System.Boolean   instance.SetPropertyByName2(SName, DValue, BValue) ``` | |

| C# |  |
| --- | --- |
| ``` void SetPropertyByName2(     System.string SName,    System.double DValue,    System.bool BValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetPropertyByName2(  &   System.String^ SName, &   System.double DValue, &   System.bool BValue ) ``` | |

#### Parameters

*SName*
:   Property name; for example, 'EX' for Elastic modulus, 'NUXY' for Poisson's ratio, etc.

*DValue*
:   Value of material property

*BValue*
:   -1 or true if temperature dependent, 0 or false if not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::SetPropertyByName2.

# ![](dotnetimages/collapse.gif)Remarks

Specify BValue as a boolean or integer: true = -1, false = 0.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04