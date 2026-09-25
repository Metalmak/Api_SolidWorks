<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~SilentFind.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SilentFind Method (IEdmFindUser) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) : SilentFind Method (IEdmFindUser) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Silently searches for users with search criteria specified by [IEdmFindUser::SetPropt](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~SetPropt.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SilentFind() ``` | |

| C# |  |
| --- | --- |
| ``` void SilentFind() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SilentFind(); ``` | |

# ![](dotnetimages/collapse.gif)Example

See the example for [IEdmFindUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html).

# ![](dotnetimages/collapse.gif)Remarks

The result of the search is returned in the property, [IEdmFindUser.Result](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~Result.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html)

[IEdmFindUser Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013