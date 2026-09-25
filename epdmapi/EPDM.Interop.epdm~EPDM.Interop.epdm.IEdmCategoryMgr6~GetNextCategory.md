<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6~GetNextCategory.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextCategory Method (IEdmCategoryMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCategoryMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6.html) : GetNextCategory Method (IEdmCategoryMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next category in the list

Gets the next category in the enumeration.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextCategory( _    ByVal poPos As IEdmPos5 _ ) As IEdmCategory6 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmCategory6 GetNextCategory(     IEdmPos5 poPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmCategory6^ GetNextCategory(  &   IEdmPos5^ poPos ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next category in the list

#### Return Value

[IEdmCategory6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategory6.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCategoryMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

To obtain the position of the first category in the list, call [IEdmCategoryMgr6::GetFirstCategoryPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6~GetFirstCategoryPosition.html).

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the categories.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: No more categories can be accessed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCategoryMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6.html)

[IEdmCategoryMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCategoryMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0