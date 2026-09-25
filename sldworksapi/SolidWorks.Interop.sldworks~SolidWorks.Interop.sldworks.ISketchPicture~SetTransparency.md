<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~SetTransparency.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetTransparency Method (ISketchPicture) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html) : SetTransparency Method (ISketchPicture) |

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

Sets the transparency parameters of this picture on the sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetTransparency( _    ByVal Style As System.Integer, _    ByVal Transparency As System.Double, _    ByVal MatchingColor As System.Integer, _    ByVal MatchingTolerance As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPicture Dim Style As System.Integer Dim Transparency As System.Double Dim MatchingColor As System.Integer Dim MatchingTolerance As System.Double Dim value As System.Boolean   value = instance.SetTransparency(Style, Transparency, MatchingColor, MatchingTolerance) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetTransparency(     System.int Style,    System.double Transparency,    System.int MatchingColor,    System.double MatchingTolerance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetTransparency(  &   System.int Style, &   System.double Transparency, &   System.int MatchingColor, &   System.double MatchingTolerance ) ``` | |

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

#### Return Value

True if transparency is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchPicture::SetTransparency.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html)

[ISketchPicture Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture_members.html)

[ISketchPicture::GetOrigin Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~GetOrigin.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0