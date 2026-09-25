<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5~GetSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetSize Method (IEdmCard5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCard5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html) : GetSize Method (IEdmCard5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*plWidth*
:   Width in pixels of this data card

*plHeight*
:   Height in pixels of this data card

Gets the size of this data card.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetSize( _    ByRef plWidth As System.Integer, _    ByRef plHeight As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSize(     out System.int plWidth,    out System.int plHeight ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSize(  &   [Out] System.int plWidth, &   [Out] System.int plHeight ) ``` | |

#### Parameters

*plWidth*
:   Width in pixels of this data card

*plHeight*
:   Height in pixels of this data card

# ![](dotnetimages/collapse.gif)Example

[Get Card Control Information (VB.NET)](Get_Card_Control_Info_Example_VBNET.htm)

[Get Card Control Information (C#)](Get_Card_Control_Info_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCard5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5.html)

[IEdmCard5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCard5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2