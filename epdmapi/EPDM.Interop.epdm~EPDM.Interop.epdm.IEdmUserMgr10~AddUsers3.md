<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr10~AddUsers3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddUsers3 Method (IEdmUserMgr10) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr10.html) : AddUsers3 Method (IEdmUserMgr10) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoUserData*
:   Array of [EdmUserData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2.html) structures; one structure for each user

*UserType*
:   Login type of users as defined in [EdmUserType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserType.html)

Adds the specified users of the specified login type to the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddUsers3( _    ByRef ppoUserData() As EdmUserData2, _    ByVal UserType As EdmUserType _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddUsers3(     out EdmUserData2[] ppoUserData,    EdmUserType UserType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddUsers3(  &   [Out] array<EdmUserData2>^ ppoUserData, &   EdmUserType UserType ) ``` | |

#### Parameters

*ppoUserData*
:   Array of [EdmUserData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2.html) structures; one structure for each user

*UserType*
:   Login type of users as defined in [EdmUserType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserType.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUserMgr10](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr10.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmUserMgr7::AddUsers2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddUsers2.html) by providing the ability to add users by type to the vault.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr10 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr10.html)

[IEdmUserMgr10 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr10_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2019