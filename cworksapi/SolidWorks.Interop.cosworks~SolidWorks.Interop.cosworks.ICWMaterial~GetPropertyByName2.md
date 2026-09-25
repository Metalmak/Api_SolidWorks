<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~GetPropertyByName2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPropertyByName2 Method (ICWMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html) : GetPropertyByName2 Method (ICWMaterial) |

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
:   -1 or true if temperature dependent, 0 or false if not (see **Remarks**)

Gets the value of the material property by the property name.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPropertyByName2( _    ByVal NUnit As System.Integer, _    ByVal SName As System.String, _    ByRef BTempDependent As System.Boolean _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMaterial Dim NUnit As System.Integer Dim SName As System.String Dim BTempDependent As System.Boolean Dim value As System.Double   value = instance.GetPropertyByName2(NUnit, SName, BTempDependent) ``` | |

| C# |  |
| --- | --- |
| ``` System.double GetPropertyByName2(     System.int NUnit,    System.string SName,    out System.bool BTempDependent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double GetPropertyByName2(  &   System.int NUnit, &   System.String^ SName, &   [Out] System.bool BTempDependent ) ``` | |

#### Parameters

*NUnit*
:   Unit system as defined in [swsUnitSystem\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnitSystem_e.html)

*SName*
:   Property name; for example, 'EX' for Elastic modulus, 'NUXY' for Poisson's ratio, etc.

*BTempDependent*
:   -1 or true if temperature dependent, 0 or false if not (see **Remarks**)

#### Return Value

Value of material property

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMaterial::GetPropertyByName2.

# ![](dotnetimages/collapse.gif)Remarks

This method returns a boolean or integer in out parameter BTempDependent, depending on its prior declaration.

If out parameter BTempDependent is cast as a:

* Boolean, true or false is returned.* Long or integer, -1 (=true) or 0 (=false) is returned.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMaterial Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial.html)

[ICWMaterial Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2021 SP04