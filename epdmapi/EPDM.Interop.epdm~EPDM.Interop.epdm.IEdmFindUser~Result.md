<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~Result.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Result Property (IEdmFindUser) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) : Result Property (IEdmFindUser) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the result of the last search for users.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property Result As IEdmEnum ``` | |

| C# |  |
| --- | --- |
| ``` IEdmEnum Result {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property IEdmEnum^ Result {    IEdmEnum^ get(); } ``` | |

#### Property Value

[IEdmEnum](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnum.html) (see Remarks)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFindUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

If [IEdmFindUser::ShowFindUI](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~ShowFindUI.html) is called, this property contains only the users that were selected in the search dialog box's result list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html)

[IEdmFindUser Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013