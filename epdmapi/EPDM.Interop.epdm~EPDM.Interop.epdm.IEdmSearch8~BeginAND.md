<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8~BeginAND.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| BeginAND Method (IEdmSearch8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSearch8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8.html) : BeginAND Method (IEdmSearch8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Begins boolean AND operation.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub BeginAND() ``` | |

| C# |  |
| --- | --- |
| ``` void BeginAND() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void BeginAND(); ``` | |

# ![](dotnetimages/collapse.gif)Example

See the [IEdmSearch8](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, call [IEdmSearch8::AddVariable2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8~AddVariable2.html) multiple times to further constrain the search.

Use [IEdmSearch8::EndAND](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8~EndAND.html) to end the AND operation.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSearch8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8.html)

[IEdmSearch8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSearch8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018