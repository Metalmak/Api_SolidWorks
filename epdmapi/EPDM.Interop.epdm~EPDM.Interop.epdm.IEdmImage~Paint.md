<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage~Paint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Paint Method (IEdmImage) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmImage Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage.html) : Paint Method (IEdmImage) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*llHDC*
:   Device context handle

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; contains the size and position where to draw the image; null to use the size and position of the image when it was created or the size and position that was passed in the last call to [IEdmImage::Reposition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage~Reposition.html)

Paints an image on the specified device context in the specified bounding rectangle.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Paint( _    ByVal llHDC As System.Long, _    Optional ByRef poDestRect As EdmRect _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Paint(     System.long llHDC,    ref EdmRect poDestRect ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Paint(  &   System.int64 llHDC, &   EdmRect% poDestRect ) ``` | |

#### Parameters

*llHDC*
:   Device context handle

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; contains the size and position where to draw the image; null to use the size and position of the image when it was created or the size and position that was passed in the last call to [IEdmImage::Reposition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage~Reposition.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmImage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmImage Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage.html)

[IEdmImage Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013