<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5~GetNextTemplate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextTemplate Method (IEdmTemplateMgr5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTemplateMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5.html) : GetNextTemplate Method (IEdmTemplateMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next template

Gets the next template in this list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextTemplate( _    ByVal poPos As IEdmPos5 _ ) As IEdmTemplate5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmTemplate5 GetNextTemplate(     IEdmPos5 poPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmTemplate5^ GetNextTemplate(  &   IEdmPos5^ poPos ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next template

#### Return Value

[IEdmTemplate5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplate5.html)

# ![](dotnetimages/collapse.gif)Example

[Execute Template (C#)](Execute_Template_Example_CSharp.htm)

[Execute Template (VB.NET)](Execute_Template_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first template, IEdmPos5. Call [IEdmTemplateMgr5::GetFirstTemplatePosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5~GetFirstTemplatePosition.html) to obtain poPos.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the templates.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmTemplate5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTemplateMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5.html)

[IEdmTemplateMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTemplateMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2