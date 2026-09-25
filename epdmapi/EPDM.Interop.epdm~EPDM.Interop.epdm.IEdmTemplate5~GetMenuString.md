<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5~GetMenuString.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetMenuString Method (IEdmTemplate5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTemplate5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5.html) : GetMenuString Method (IEdmTemplate5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the string displayed in the SOLIDWORKS PDM Professional menu for this template.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetMenuString() As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetMenuString() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetMenuString(); ``` | |

#### Return Value

Menu string

# ![](dotnetimages/collapse.gif)Example

[Execute Template (C#)](Execute_Template_Example_CSharp.htm)

[Execute Template (VB.NET)](Execute_Template_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

C++ programmers not using bstr\_t wrapper functions must free the returned string with a call to SysFreeString.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTemplate5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5.html)

[IEdmTemplate5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2