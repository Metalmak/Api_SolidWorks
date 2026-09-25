<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6~AddUsers.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddUsers Method (IEdmUserMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6.html) : AddUsers Method (IEdmUserMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoUserData*
:   Array of [EdmUserData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData.html) structures; one structure for each user

Obsolete. Superseded by [IEdmUserMgr7::AddUsers2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddUsers2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddUsers( _    ByRef ppoUserData() As EdmUserData _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddUsers(     out EdmUserData[] ppoUserData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddUsers(  &   [Out] array<EdmUserData>^ ppoUserData ) ``` | |

#### Parameters

*ppoUserData*
:   Array of [EdmUserData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData.html) structures; one structure for each user

# ![](dotnetimages/collapse.gif)Remarks

This method is superseded by [IEdmUserMgr7::AddUsers2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddUsers2.html) which allows you to specify system permissions.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6.html)

[IEdmUserMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007