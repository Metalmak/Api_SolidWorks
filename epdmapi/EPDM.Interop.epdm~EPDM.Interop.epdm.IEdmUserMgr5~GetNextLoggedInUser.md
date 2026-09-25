<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5~GetNextLoggedInUser.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextLoggedInUser Method (IEdmUserMgr5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html) : GetNextLoggedInUser Method (IEdmUserMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position in the enumeration of the next logged-in user

*pbsUserName*
:   Name of the logged-in user (see **Remarks**)

*pbsComputerName*
:   Name of the computer in which the user is logged (see **Remarks**)

*pbsVaultName*
:   Name of the vault in which the user is logged (see **Remarks**)

*poLoginTime*
:   Date and time of the moment when the user logged in to the vault (see **Remarks**)

Gets information about the next logged-in user in an enumeration of all logged-in users in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetNextLoggedInUser( _    ByVal poPos As IEdmPos5, _    ByRef pbsUserName As System.String, _    ByRef pbsComputerName As System.String, _    ByRef pbsVaultName As System.String, _    ByRef poLoginTime As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetNextLoggedInUser(     IEdmPos5 poPos,    out System.string pbsUserName,    out System.string pbsComputerName,    out System.string pbsVaultName,    out System.object poLoginTime ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetNextLoggedInUser(  &   IEdmPos5^ poPos, &   [Out] System.String^ pbsUserName, &   [Out] System.String^ pbsComputerName, &   [Out] System.String^ pbsVaultName, &   [Out] System.Object^ poLoginTime ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position in the enumeration of the next logged-in user

*pbsUserName*
:   Name of the logged-in user (see **Remarks**)

*pbsComputerName*
:   Name of the computer in which the user is logged (see **Remarks**)

*pbsVaultName*
:   Name of the vault in which the user is logged (see **Remarks**)

*poLoginTime*
:   Date and time of the moment when the user logged in to the vault (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Create New Vault (VB.NET)](Create_New_Vault_Example_VBNET.htm)

[Create New Vault (C#)](Create_New_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first logged-in user in the list, IEdmPos5. Call [IEdmUserMgr5::GetFirstLoggedInUserPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5~GetFirstLoggedInUserPosition.html) to obtain poPos.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the logged-in users in the list.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ users must free the strings returned in pbsUserName, pbsComputerName, and pbsVaultName with a call to SysFreeString. C++ users must initialize the VARIANT struct in poLoginTime with a call to VariantInit before calling this method. After the method has returned, the contents of the VARIANT struct must be freed by calling VariantClear.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5.html)

[IEdmUserMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2