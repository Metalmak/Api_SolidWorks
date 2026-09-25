<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5~GetPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetPosition Method (IEdmCardControl5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardControl5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html) : GetPosition Method (IEdmCardControl5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*plX*
:   X-coordinate of the top-left corner of the control

*plY*
:   Y-coordinate of the top-left corner of the control

*plWidth*
:   Width of the control in pixels

*plHeight*
:   Height of the control in pixels

Gets the dimensions and position of this control.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetPosition( _    ByRef plX As System.Integer, _    ByRef plY As System.Integer, _    ByRef plWidth As System.Integer, _    ByRef plHeight As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetPosition(     out System.int plX,    out System.int plY,    out System.int plWidth,    out System.int plHeight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetPosition(  &   [Out] System.int plX, &   [Out] System.int plY, &   [Out] System.int plWidth, &   [Out] System.int plHeight ) ``` | |

#### Parameters

*plX*
:   X-coordinate of the top-left corner of the control

*plY*
:   Y-coordinate of the top-left corner of the control

*plWidth*
:   Width of the control in pixels

*plHeight*
:   Height of the control in pixels

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardControl6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardControl5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html)

[IEdmCardControl5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2