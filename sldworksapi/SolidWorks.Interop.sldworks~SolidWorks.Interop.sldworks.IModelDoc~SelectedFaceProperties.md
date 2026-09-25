<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc~SelectedFaceProperties.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SelectedFaceProperties Method (IModelDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html) : SelectedFaceProperties Method (IModelDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*RgbColor*

*Ambient*

*Diffuse*

*Specular*

*Shininess*

*Transparency*

*Emission*

*UsePartProps*

*FaceName*

Obsolete. Superseded by [IModelDoc2::SelectedFaceProperties](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~SelectedFaceProperties.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SelectedFaceProperties( _    ByVal RgbColor As System.Integer, _    ByVal Ambient As System.Double, _    ByVal Diffuse As System.Double, _    ByVal Specular As System.Double, _    ByVal Shininess As System.Double, _    ByVal Transparency As System.Double, _    ByVal Emission As System.Double, _    ByVal UsePartProps As System.Boolean, _    ByVal FaceName As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc Dim RgbColor As System.Integer Dim Ambient As System.Double Dim Diffuse As System.Double Dim Specular As System.Double Dim Shininess As System.Double Dim Transparency As System.Double Dim Emission As System.Double Dim UsePartProps As System.Boolean Dim FaceName As System.String Dim value As System.Boolean   value = instance.SelectedFaceProperties(RgbColor, Ambient, Diffuse, Specular, Shininess, Transparency, Emission, UsePartProps, FaceName) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SelectedFaceProperties(     System.int RgbColor,    System.double Ambient,    System.double Diffuse,    System.double Specular,    System.double Shininess,    System.double Transparency,    System.double Emission,    System.bool UsePartProps,    System.string FaceName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SelectedFaceProperties(  &   System.int RgbColor, &   System.double Ambient, &   System.double Diffuse, &   System.double Specular, &   System.double Shininess, &   System.double Transparency, &   System.double Emission, &   System.bool UsePartProps, &   System.String^ FaceName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*RgbColor*

*Ambient*

*Diffuse*

*Specular*

*Shininess*

*Transparency*

*Emission*

*UsePartProps*

*FaceName*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc::SelectedFaceProperties.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc.html)

[IModelDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc_members.html)