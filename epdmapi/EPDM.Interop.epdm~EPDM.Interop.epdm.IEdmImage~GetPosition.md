<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage~GetPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetPosition Method (IEdmImage) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmImage Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage.html) : GetPosition Method (IEdmImage) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; contains the size and position where to draw the image

Gets the bounding rectangle where the image is drawn.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetPosition( _    ByRef poDestRect As EdmRect _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetPosition(     out EdmRect poDestRect ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetPosition(  &   [Out] EdmRect poDestRect ) ``` | |

#### Parameters

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; contains the size and position where to draw the image

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmImage Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage.html)

[IEdmImage Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013