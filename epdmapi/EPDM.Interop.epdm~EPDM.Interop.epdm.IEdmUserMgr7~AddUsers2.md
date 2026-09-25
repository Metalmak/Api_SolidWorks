<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7~AddUsers2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddUsers2 Method (IEdmUserMgr7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html) : AddUsers2 Method (IEdmUserMgr7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoUserData*
:   Array of [EdmUserData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2.html) structures; one structure for each user

Obsolete. Superseded by [IEdmUserMgr10::AddUsers3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr10~AddUsers3.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddUsers2( _    ByRef ppoUserData() As EdmUserData2 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddUsers2(     out EdmUserData2[] ppoUserData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddUsers2(  &   [Out] array<EdmUserData2>^ ppoUserData ) ``` | |

#### Parameters

*ppoUserData*
:   Array of [EdmUserData2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserData2.html) structures; one structure for each user

# ![](dotnetimages/collapse.gif)Example

[Add Users (VB.NET)](Add_Users_Example_VBNET.htm)

[Add Users (C#)](Add_Users_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmUserMgr6::AddUsers](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr6~AddUsers.html) by providing the ability to specify permissions for added users.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7.html)

[IEdmUserMgr7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010