<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetAdvancedSpotLightProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetAdvancedSpotLightProperties Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : GetAdvancedSpotLightProperties Method (IModelDocExtension) |

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

Gets the attenuation-related, advanced properties for the specified SOLIDWORKS spot light in this model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetAdvancedSpotLightProperties( _    ByVal Name As System.String, _    ByRef Exponent As System.Double, _    ByRef AttenuationConst As System.Double, _    ByRef AttenuationLinear As System.Double, _    ByRef AttenuationQuad As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Name As System.String Dim Exponent As System.Double Dim AttenuationConst As System.Double Dim AttenuationLinear As System.Double Dim AttenuationQuad As System.Double   instance.GetAdvancedSpotLightProperties(Name, Exponent, AttenuationConst, AttenuationLinear, AttenuationQuad) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAdvancedSpotLightProperties(     System.string Name,    out System.double Exponent,    out System.double AttenuationConst,    out System.double AttenuationLinear,    out System.double AttenuationQuad ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAdvancedSpotLightProperties(  &   System.String^ Name, &   [Out] System.double Exponent, &   [Out] System.double AttenuationConst, &   [Out] System.double AttenuationLinear, &   [Out] System.double AttenuationQuad ) ``` | |

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

See ModelDocExtension::GetAdvancedSpotLightProperties.

# ![](dotnetimages/collapse.gif)Example

[Get Advanced Properties of Spot Light (VBA)](Get_Advanced_Properties_of_Spot_Light_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

See the SOLIDWORKS Help for more information about the advanced properties of spot lights.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0