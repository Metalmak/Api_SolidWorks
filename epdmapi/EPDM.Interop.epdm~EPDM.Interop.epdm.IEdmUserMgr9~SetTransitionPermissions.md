<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9~SetTransitionPermissions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetTransitionPermissions Method (IEdmUserMgr9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9.html) : SetTransitionPermissions Method (IEdmUserMgr9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPermissions*
:   Array of [EdmTransitionPermission](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission.html) structures; one structure for each permission assignment

Sets transition permissions.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetTransitionPermissions( _    ByVal poPermissions() As EdmTransitionPermission _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetTransitionPermissions(     EdmTransitionPermission[] poPermissions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetTransitionPermissions(  &   array<EdmTransitionPermission>^ poPermissions ) ``` | |

#### Parameters

*poPermissions*
:   Array of [EdmTransitionPermission](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTransitionPermission.html) structures; one structure for each permission assignment

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The logged-in user lacks the [EdmSysPerm](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysPerm.html).EdmSysPerm\_EditUserMgr permission.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9.html)

[IEdmUserMgr9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9_members.html)

[IEdmUserMgr9::GetTransitionPermissions Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr9~GetTransitionPermissions.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017