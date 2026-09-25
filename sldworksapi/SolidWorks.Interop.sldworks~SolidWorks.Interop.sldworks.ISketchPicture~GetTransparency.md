<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~GetTransparency.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetTransparency Method (ISketchPicture) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html) : GetTransparency Method (ISketchPicture) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Style*
:   Style as defined by swSketchPictureTransparencyStyle\_e

*Transparency*
:   * 0 = opaque* 1 = transparent

    describing the relative transparency depending on the value of Style

*MatchingColor*
:   RGB color used as the transparent color when Style is swSketchPictureTransparencyUserDefined

*MatchingTolerance*
:   * 0 = exact match* 1 = less exact match

    indicating how closely MatchingColor must be to be considered a transparent color when Style is swSketchPictureTransparencyUserDefined

Gets transparency parameters for this picture.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetTransparency( _    ByRef Style As System.Integer, _    ByRef Transparency As System.Double, _    ByRef MatchingColor As System.Integer, _    ByRef MatchingTolerance As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPicture Dim Style As System.Integer Dim Transparency As System.Double Dim MatchingColor As System.Integer Dim MatchingTolerance As System.Double   instance.GetTransparency(Style, Transparency, MatchingColor, MatchingTolerance) ``` | |

| C# |  |
| --- | --- |
| ``` void GetTransparency(     out System.int Style,    out System.double Transparency,    out System.int MatchingColor,    out System.double MatchingTolerance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetTransparency(  &   [Out] System.int Style, &   [Out] System.double Transparency, &   [Out] System.int MatchingColor, &   [Out] System.double MatchingTolerance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Style*
:   Style as defined by swSketchPictureTransparencyStyle\_e

*Transparency*
:   * 0 = opaque* 1 = transparent

    describing the relative transparency depending on the value of Style

*MatchingColor*
:   RGB color used as the transparent color when Style is swSketchPictureTransparencyUserDefined

*MatchingTolerance*
:   * 0 = exact match* 1 = less exact match

    indicating how closely MatchingColor must be to be considered a transparent color when Style is swSketchPictureTransparencyUserDefined

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchPicture::GetTransparency.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html)

[ISketchPicture Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0