<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5~Draw.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Draw Method (IEdmBitmap5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBitmap5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5.html) : Draw Method (IEdmBitmap5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lWnd*
:   Handle of window in which to draw the bitmap image

*lX*
:   X-coordinate in pixels where to position upper-left corner of image ; default is 0

*lY*
:   Y-coordinate in pixels where to position upper-left corner of image; default is 0

*lWidth*
:   Width in pixels of the drawn image; 0 for source image width

*lHeight*
:   Height in pixels of the drawn image; 0 for source image height

Draws this bitmap image in a window.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Draw( _    ByVal lWnd As System.Integer, _    Optional ByVal lX As System.Integer, _    Optional ByVal lY As System.Integer, _    Optional ByVal lWidth As System.Integer, _    Optional ByVal lHeight As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Draw(     System.int lWnd,    System.int lX,    System.int lY,    System.int lWidth,    System.int lHeight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Draw(  &   System.int lWnd, &   System.int lX, &   System.int lY, &   System.int lWidth, &   System.int lHeight ) ``` | |

#### Parameters

*lWnd*
:   Handle of window in which to draw the bitmap image

*lX*
:   X-coordinate in pixels where to position upper-left corner of image ; default is 0

*lY*
:   Y-coordinate in pixels where to position upper-left corner of image; default is 0

*lWidth*
:   Width in pixels of the drawn image; 0 for source image width

*lHeight*
:   Height in pixels of the drawn image; 0 for source image height

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBitmap5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBitmap5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5.html)

[IEdmBitmap5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBitmap5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2