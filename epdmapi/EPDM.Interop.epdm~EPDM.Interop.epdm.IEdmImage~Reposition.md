<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage~Reposition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Reposition Method (IEdmImage) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmImage Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage.html) : Reposition Method (IEdmImage) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; size and position where to draw the image

*eRefresh*
:   Type of refresh of the window as defined in [EdmRepaintType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRepaintType.html)

Changes the bounding rectangle where to draw the image.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Reposition( _    ByRef poDestRect As EdmRect, _    Optional ByVal eRefresh As EdmRepaintType _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Reposition(     ref EdmRect poDestRect,    EdmRepaintType eRefresh ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Reposition(  &   EdmRect% poDestRect, &   EdmRepaintType eRefresh ) ``` | |

#### Parameters

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; size and position where to draw the image

*eRefresh*
:   Type of refresh of the window as defined in [EdmRepaintType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRepaintType.html)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmImage Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage.html)

[IEdmImage Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013