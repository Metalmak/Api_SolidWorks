<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5~GetUser.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetUser Method (IEdmUserMgr5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html) : GetUser Method (IEdmUserMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poIdOrName*
:   Id or name of user to get

Gets a user with the specified name or ID.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetUser( _    ByRef poIdOrName As System.Object _ ) As IEdmUser5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmUser5 GetUser(     ref System.object poIdOrName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmUser5^ GetUser(  &   System.Object^% poIdOrName ) ``` | |

#### Parameters

*poIdOrName*
:   Id or name of user to get

#### Return Value

[IEdmUser5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser5.html)

# ![](dotnetimages/collapse.gif)Example

[Add Folder (VB.NET)](Add_Folder_Example_VBNET.htm)

[Add Folder (C#)](Add_Folder_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

C++ users must release the returned interface, IEdmUser5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The poIdOrName argument contains an unknown user name. ppoRetUser contains null when this happens in C++.* E\_EDM\_INVALID\_ID: The poIdOrName argument contains an invalid ID.* E\_EDM\_DATABASE\_ACCESS: Returned only for invalid IDs in SOLIDWORKS PDM Professional 5.2.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html)

[IEdmUserMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2