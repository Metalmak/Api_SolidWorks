<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5~GetFirstTemplatePosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstTemplatePosition Method (IEdmTemplateMgr5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTemplateMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5.html) : GetFirstTemplatePosition Method (IEdmTemplateMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of the templates installed in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstTemplatePosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstTemplatePosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstTemplatePosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first installed template

# ![](dotnetimages/collapse.gif)Example

[Execute Template (C#)](Execute_Template_Example_CSharp.htm)

[Execute Template (VB.NET)](Execute_Template_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the position of the first template to [IEdmTemplateMgr5::GetNextTemplate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5~GetNextTemplate.html) to get the first template in this list. Then call IEdmTemplateMgr5::GetNextTemplate repeatedly to get the rest of the templates in this list.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTemplateMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5.html)

[IEdmTemplateMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2