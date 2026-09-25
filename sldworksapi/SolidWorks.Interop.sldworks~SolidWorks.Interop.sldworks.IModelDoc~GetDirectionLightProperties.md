<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~GetDirectionLightProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDirectionLightProperties Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : GetDirectionLightProperties Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*

*Ambient*

*Diffuse*

*Specular*

*Colour*

*Enabled*

*Fixed*

*X*

*Y*

*Z*

Obsolete. Superseded by [IModelDoc2::GetDirectionLightProperties](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~GetDirectionLightProperties.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDirectionLightProperties( _    ByVal Name As System.String, _    ByRef Ambient As System.Double, _    ByRef Diffuse As System.Double, _    ByRef Specular As System.Double, _    ByRef Colour As System.Integer, _    ByRef Enabled As System.Boolean, _    ByRef Fixed As System.Boolean, _    ByRef X As System.Double, _    ByRef Y As System.Double, _    ByRef Z As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim Name As System.String Dim Ambient As System.Double Dim Diffuse As System.Double Dim Specular As System.Double Dim Colour As System.Integer Dim Enabled As System.Boolean Dim Fixed As System.Boolean Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As System.Boolean   value = instance.GetDirectionLightProperties(Name, Ambient, Diffuse, Specular, Colour, Enabled, Fixed, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetDirectionLightProperties(     System.string Name,    ref System.double Ambient,    ref System.double Diffuse,    ref System.double Specular,    ref System.int Colour,    ref System.bool Enabled,    ref System.bool Fixed,    ref System.double X,    ref System.double Y,    ref System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetDirectionLightProperties(  &   System.String^ Name, &   System.double% Ambient, &   System.double% Diffuse, &   System.double% Specular, &   System.int% Colour, &   System.bool% Enabled, &   System.bool% Fixed, &   System.double% X, &   System.double% Y, &   System.double% Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*

*Ambient*

*Diffuse*

*Specular*

*Colour*

*Enabled*

*Fixed*

*X*

*Y*

*Z*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::GetDirectionLightProperties.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)