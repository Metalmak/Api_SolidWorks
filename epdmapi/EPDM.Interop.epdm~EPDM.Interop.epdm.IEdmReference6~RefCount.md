<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference6~RefCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RefCount Property (IEdmReference6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmReference6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference6.html) : RefCount Property (IEdmReference6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the number of times the referenced file is included by the referencing file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property RefCount As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int RefCount {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int RefCount {    System.int get(); } ``` | |

#### Property Value

Number of times the referenced file is included by the referencing file (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

This property is 0 if the file format does not allow SOLIDWORKS PDM Professional to access the information.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmReference6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference6.html)

[IEdmReference6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference6_members.html)

[IEdmReference8::RefCountEdited Property ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference8~RefCountEdited.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.0 of SOLIDWORKS PDM Professional