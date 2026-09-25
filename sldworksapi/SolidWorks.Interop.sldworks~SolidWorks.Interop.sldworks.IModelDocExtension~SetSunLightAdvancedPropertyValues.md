<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetSunLightAdvancedPropertyValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSunLightAdvancedPropertyValues Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : SetSunLightAdvancedPropertyValues Method (IModelDocExtension) |

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

Sets the specified sunlight advanced properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSunLightAdvancedPropertyValues( _    ByVal Haze As System.Double, _    ByVal SunDiameter As System.Double, _    ByVal GroundAlbedo As System.Integer, _    ByVal SkyGamma As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Haze As System.Double Dim SunDiameter As System.Double Dim GroundAlbedo As System.Integer Dim SkyGamma As System.Double Dim value As System.Boolean   value = instance.SetSunLightAdvancedPropertyValues(Haze, SunDiameter, GroundAlbedo, SkyGamma) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSunLightAdvancedPropertyValues(     System.double Haze,    System.double SunDiameter,    System.int GroundAlbedo,    System.double SkyGamma ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSunLightAdvancedPropertyValues(  &   System.double Haze, &   System.double SunDiameter, &   System.int GroundAlbedo, &   System.double SkyGamma ) ``` | |

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

See ModelDocExtension::SetSunLightAdvancedPropertyValues.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, call [IModelDocExtension::UpdateSunLight](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~UpdateSunLight.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::GetSunLightAdvancedPropertyValues Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetSunLightAdvancedPropertyValues.html)

[IModelDocExtension::SetSunLightSourcePropertyValues Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetSunLightSourcePropertyValues.html)

[IModelDocExtension::SunLightInformation Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SunLightInformation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0