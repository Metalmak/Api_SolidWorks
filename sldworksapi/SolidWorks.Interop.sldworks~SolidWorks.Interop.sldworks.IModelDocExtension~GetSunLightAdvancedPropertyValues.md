<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSunLightAdvancedPropertyValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSunLightAdvancedPropertyValues Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetSunLightAdvancedPropertyValues Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Haze*
:   0.0 <= Haze setting < = 1.0

*SunDiameter*
:   0.01 < = sun diameter visible in the scene <= 21474836.47

*GroundAlbedo*
:   RGB color reflected from the ground upwards

*SkyGamma*
:   0.1 <= visible sky Output Gamma <= 100.0

Gets the specified sunlight advanced properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSunLightAdvancedPropertyValues( _    ByRef Haze As System.Double, _    ByRef SunDiameter As System.Double, _    ByRef GroundAlbedo As System.Integer, _    ByRef SkyGamma As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Haze As System.Double Dim SunDiameter As System.Double Dim GroundAlbedo As System.Integer Dim SkyGamma As System.Double Dim value As System.Boolean   value = instance.GetSunLightAdvancedPropertyValues(Haze, SunDiameter, GroundAlbedo, SkyGamma) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetSunLightAdvancedPropertyValues(     out System.double Haze,    out System.double SunDiameter,    out System.int GroundAlbedo,    out System.double SkyGamma ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetSunLightAdvancedPropertyValues(  &   [Out] System.double Haze, &   [Out] System.double SunDiameter, &   [Out] System.int GroundAlbedo, &   [Out] System.double SkyGamma ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Haze*
:   0.0 <= Haze setting < = 1.0

*SunDiameter*
:   0.01 < = sun diameter visible in the scene <= 21474836.47

*GroundAlbedo*
:   RGB color reflected from the ground upwards

*SkyGamma*
:   0.1 <= visible sky Output Gamma <= 100.0

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::GetSunLightAdvancedPropertyValues.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Sunlight Source Property Values (VBA)](Get_and_Set_Sunlight_Source_Property_Values_Example_VB.htm)

[Get and Set Sunlight Source Property Values (VB.NET)](Get_and_Set_Sunlight_Source_Property_Values_Example_VBNET.htm)

[Get and Set Sunlight Source Property Values (C#)](Get_and_Set_Sunlight_Source_Property_Values_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::SetSunLightAdvancedPropertyValues Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetSunLightAdvancedPropertyValues.html)

[IModelDocExtension::UpdateSunLight Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpdateSunLight.html)

[IModelDocExtension::GetSunLightSourcePropertyValues Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSunLightSourcePropertyValues.html)

[IModelDocExtension::SunLightInformation Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SunLightInformation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0