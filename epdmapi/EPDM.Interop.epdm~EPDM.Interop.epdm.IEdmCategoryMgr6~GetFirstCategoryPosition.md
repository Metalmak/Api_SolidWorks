<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6~GetFirstCategoryPosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstCategoryPosition Method (IEdmCategoryMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCategoryMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6.html) : GetFirstCategoryPosition Method (IEdmCategoryMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of the categories in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstCategoryPosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstCategoryPosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstCategoryPosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first category in the list

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCategoryMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, call [IEdmCategoryMgr6::GetNextCategory](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6~GetNextCategory.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCategoryMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6.html)

[IEdmCategoryMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0