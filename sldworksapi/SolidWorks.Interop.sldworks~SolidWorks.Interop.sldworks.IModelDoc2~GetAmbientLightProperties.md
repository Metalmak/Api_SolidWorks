<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetAmbientLightProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetAmbientLightProperties Method (IModelDoc2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : GetAmbientLightProperties Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*
:   Light name

*Ambient*
:   Light source ambient value

*Diffuse*
:   Light source diffuse value

*Specular*
:   Light source specular value

*Colour*
:   COLORREF color value

*Enabled*
:   True if a light is enabled, false if not

*Fixed*
:   True if a light is fixed, false if not

Gets the ambient light properties for this model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAmbientLightProperties( _    ByVal Name As System.String, _    ByRef Ambient As System.Double, _    ByRef Diffuse As System.Double, _    ByRef Specular As System.Double, _    ByRef Colour As System.Integer, _    ByRef Enabled As System.Boolean, _    ByRef Fixed As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim Name As System.String Dim Ambient As System.Double Dim Diffuse As System.Double Dim Specular As System.Double Dim Colour As System.Integer Dim Enabled As System.Boolean Dim Fixed As System.Boolean Dim value As System.Boolean   value = instance.GetAmbientLightProperties(Name, Ambient, Diffuse, Specular, Colour, Enabled, Fixed) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetAmbientLightProperties(     System.string Name,    ref System.double Ambient,    ref System.double Diffuse,    ref System.double Specular,    ref System.int Colour,    ref System.bool Enabled,    ref System.bool Fixed ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetAmbientLightProperties(  &   System.String^ Name, &   System.double% Ambient, &   System.double% Diffuse, &   System.double% Specular, &   System.int% Colour, &   System.bool% Enabled, &   System.bool% Fixed ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*
:   Light name

*Ambient*
:   Light source ambient value

*Diffuse*
:   Light source diffuse value

*Specular*
:   Light source specular value

*Colour*
:   COLORREF color value

*Enabled*
:   True if a light is enabled, false if not

*Fixed*
:   True if a light is fixed, false if not

#### Return Value

True if light properties determined without a problem, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::GetAmbientLightProperties.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::SetAmbientLightProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetAmbientLightProperties.html)

[IModelDoc2::GetDirectionLightProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetDirectionLightProperties.html)

[IModelDoc2::GetPointLightProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetPointLightProperties.html)

[IModelDoc2::GetSpotlightProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~GetSpotlightProperties.html)

[IModelDoc2::SetDirectionLightProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetDirectionLightProperties.html)

[IModelDoc2::SetPointLightProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetPointLightProperties.html)

[IModelDoc2::SetSpotlightProperties Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetSpotlightProperties.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0