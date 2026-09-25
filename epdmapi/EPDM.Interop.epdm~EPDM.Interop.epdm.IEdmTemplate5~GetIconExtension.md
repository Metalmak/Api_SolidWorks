<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5~GetIconExtension.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetIconExtension Method (IEdmTemplate5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTemplate5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5.html) : GetIconExtension Method (IEdmTemplate5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the file extension for the icon registered with this template.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetIconExtension() As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetIconExtension() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetIconExtension(); ``` | |

#### Return Value

File extension of the icon registered with this template

# ![](dotnetimages/collapse.gif)Remarks

Templates are listed with a menu string and, optionally, an icon in SOLIDWORKS PDM Professional's menus and list controls. The file extension retrieved maps to the registered icon for the Windows file type of this template.

C++ programmers not using bstr\_t wrapper functions must free the returned string with a call to SysFreeString.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTemplate5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5.html)

[IEdmTemplate5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2