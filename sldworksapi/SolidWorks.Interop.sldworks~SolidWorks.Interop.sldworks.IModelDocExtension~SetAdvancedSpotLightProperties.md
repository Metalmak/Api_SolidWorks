<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetAdvancedSpotLightProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetAdvancedSpotLightProperties Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : SetAdvancedSpotLightProperties Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   SOLIDWORKS light source name

*Exponent*
:   Attenuation exponent

*AttenuationConst*
:   Constant attenuation factor

*AttenuationLinear*
:   Linear attenuation factor

*AttenuationQuad*
:   Quadratic attenuation factor

Sets the attenuation-related, advanced properties for the specified SOLIDWORKS spot light in this model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetAdvancedSpotLightProperties( _    ByVal Name As System.String, _    ByVal Exponent As System.Double, _    ByVal AttenuationConst As System.Double, _    ByVal AttenuationLinear As System.Double, _    ByVal AttenuationQuad As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Name As System.String Dim Exponent As System.Double Dim AttenuationConst As System.Double Dim AttenuationLinear As System.Double Dim AttenuationQuad As System.Double   instance.SetAdvancedSpotLightProperties(Name, Exponent, AttenuationConst, AttenuationLinear, AttenuationQuad) ``` | |

| C# |  |
| --- | --- |
| ``` void SetAdvancedSpotLightProperties(     System.string Name,    System.double Exponent,    System.double AttenuationConst,    System.double AttenuationLinear,    System.double AttenuationQuad ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetAdvancedSpotLightProperties(  &   System.String^ Name, &   System.double Exponent, &   System.double AttenuationConst, &   System.double AttenuationLinear, &   System.double AttenuationQuad ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   SOLIDWORKS light source name

*Exponent*
:   Attenuation exponent

*AttenuationConst*
:   Constant attenuation factor

*AttenuationLinear*
:   Linear attenuation factor

*AttenuationQuad*
:   Quadratic attenuation factor

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::SetAdvancedSpotLightProperties.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0