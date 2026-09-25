<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6~AddGroups.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddGroups Method (IEdmUserMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6.html) : AddGroups Method (IEdmUserMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoGroupData*
:   Array of [EdmGroupData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData.html) structures; one structure for each user group

Obsolete. Superseded by [IEdmUserMgr7::AddGroups2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddGroups2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddGroups( _    ByRef ppoGroupData() As EdmGroupData _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddGroups(     out EdmGroupData[] ppoGroupData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddGroups(  &   [Out] array<EdmGroupData>^ ppoGroupData ) ``` | |

#### Parameters

*ppoGroupData*
:   Array of [EdmGroupData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGroupData.html) structures; one structure for each user group

# ![](dotnetimages/collapse.gif)Remarks

This method is superseded by [IEdmUserMgr7::AddGroups2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddGroups2.html) which allows you to specify system permissions.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6.html)

[IEdmUserMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007