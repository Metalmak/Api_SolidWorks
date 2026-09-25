<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetPropertyByName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPropertyByName Method (ICWMaterial) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : GetPropertyByName Method (ICWMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NUnit*
:   Unit system as defined in [swsUnitSystem\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnitSystem_e.html)

*SName*
:   Property name; for example, 'EX' for Elastic modulus, 'NUXY' for Poisson's ratio, etc.

*BTempDependent*
:   True if temperature dependent, false if not

Obsolete. Superseded by er[ICWMaterial::GetPropertyByName2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetPropertyByName2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPropertyByName( _    ByVal NUnit As System.Integer, _    ByVal SName As System.String, _    ByRef BTempDependent As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim NUnit As System.Integer Dim SName As System.String Dim BTempDependent As System.Integer Dim value As System.Double   value = instance.GetPropertyByName(NUnit, SName, BTempDependent) ``` | |

| C# |  |
| --- | --- |
| ``` System.double GetPropertyByName(     System.int NUnit,    System.string SName,    out System.int BTempDependent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double GetPropertyByName(  &   System.int NUnit, &   System.String^ SName, &   [Out] System.int BTempDependent ) ``` | |

#### Parameters

*NUnit*
:   Unit system as defined in [swsUnitSystem\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnitSystem_e.html)

*SName*
:   Property name; for example, 'EX' for Elastic modulus, 'NUXY' for Poisson's ratio, etc.

*BTempDependent*
:   True if temperature dependent, false if not

#### Return Value

Value of material property

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::GetPropertyByName.

# ![](dotnetimages/collapse.gif)Example

[Apply Material to Bodies (C#)](Apply_Material_to_Bodies_Example_CSharp.htm)

[Apply Material to Bodies (VB.NET)](Apply_Material_to_Bodies_Example_VBNET.htm)

[Apply Material to Bodies (VBA)](Apply_Material_to_Bodies_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

[ICWMaterial::SetPropertyByName Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~SetPropertyByName.html)

[ICWMaterial::Count Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~Count.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0