<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~Recursive.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Recursive Property (IEdmSearch5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html) : Recursive Property (IEdmSearch5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to search recursively in subfolders.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Property Recursive As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Recursive {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool Recursive {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

True to search recursively in subfolders, false to search only in the folder specified by [IEdmSearch5::StartFolderID](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5~StartFolderID.html)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5.html)

[IEdmSearch5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2