<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetErrorString.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetErrorString Method (IEdmVault5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : GetErrorString Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lError*
:   Error code for which to get a description

*pbsErrorName*
:   Error name as defined in [Return codes](ReturnCodes.htm); hexadecimal number if the error is unknown

*pbsDescription*
:   Description of the error

Gets the name and description for the specified error code returned by one of SOLIDWORKS PDM Professional's API methods.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetErrorString( _    ByVal lError As System.Integer, _    Optional ByRef pbsErrorName As System.String, _    Optional ByRef pbsDescription As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetErrorString(     System.int lError,    out System.string pbsErrorName,    out System.string pbsDescription ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetErrorString(  &   System.int lError, &   [Out] System.String^ pbsErrorName, &   [Out] System.String^ pbsDescription ) ``` | |

#### Parameters

*lError*
:   Error code for which to get a description

*pbsErrorName*
:   Error name as defined in [Return codes](ReturnCodes.htm); hexadecimal number if the error is unknown

*pbsDescription*
:   Description of the error

# ![](dotnetimages/collapse.gif)Example

[Batch Add Files and Folders to Vault (VB.NET)](Batch_Add_Files_and_Folders_Example_VBNET.htm)

[Batch Add Files and Folders to Vault (C#)](Batch_Add_Files_and_Folders_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

You do not have to be logged in to the vault to call this method.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

[IEdmVault11::GetErrorMessage Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorMessage.html)

[IEdmVault11::GetErrorName Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2