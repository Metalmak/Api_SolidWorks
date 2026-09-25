<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetPropertyByName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetPropertyByName Method (ICWMaterial) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : SetPropertyByName Method (ICWMaterial) |

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
:   True if temperature dependent, false if not

Obsolete. Superseded by [ICWMaterial::SetPropertyByName2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetPropertyByName2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetPropertyByName( _    ByVal SName As System.String, _    ByVal DValue As System.Double, _    ByVal BValue As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim SName As System.String Dim DValue As System.Double Dim BValue As System.Integer   instance.SetPropertyByName(SName, DValue, BValue) ``` | |

| C# |  |
| --- | --- |
| ``` void SetPropertyByName(     System.string SName,    System.double DValue,    System.int BValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetPropertyByName(  &   System.String^ SName, &   System.double DValue, &   System.int BValue ) ``` | |

#### Parameters

*SName*
:   Property name; for example, 'EX' for Elastic modulus, 'NUXY' for Poisson's ratio, etc.

*DValue*
:   Value of material property

*BValue*
:   True if temperature dependent, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::SetPropertyByName.

# ![](dotnetimages/collapse.gif)Example

[Create Nonlinear Study and Apply Materials (C#)](Create_Nonlinear_Study_and_Apply_Materials_Example_CSharp.htm)

[Create Nonlinear Study and Apply Materials (VB.NET)](Create_Nonlinear_Study_and_Apply_Materials_Example_VBNET.htm)

[Create Nonlinear Study and Apply Materials (VBA)](Create_Nonlinear_Study_and_Apply_Materials_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

[ICWMaterial::GetPropertyByName Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetPropertyByName.html)

[ICWMaterial::Count Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~Count.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0