<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMessage5~IsRead.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IsRead Property (IEdmMessage5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMessage5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMessage5.html) : IsRead Property (IEdmMessage5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets or sets whether the message has been read.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Property IsRead As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsRead {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool IsRead {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

True if the message has been read, false if not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmMessage5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMessage5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

You can only set this property to true; you cannot set it to false.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMessage5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMessage5.html)

[IEdmMessage5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMessage5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.3 of SOLIDWORKS PDM Professional