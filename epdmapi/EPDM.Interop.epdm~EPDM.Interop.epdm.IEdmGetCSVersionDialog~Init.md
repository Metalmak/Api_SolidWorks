<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetCSVersionDialog~Init.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Init Method (IEdmGetCSVersionDialog) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmGetCSVersionDialog Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetCSVersionDialog.html) : Init Method (IEdmGetCSVersionDialog) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); pointer to the vault

*lArcSrvID*
:   Archive server ID

*eError*
:   [EdmGetOpError](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpError.html); error code returned after getting coldstored version

*bsFileName*
:   Name of the file being restored from cold storage

*lDocID*
:   ID of the document being restored from cold storage

*lVersionNo*
:   Version number of the file being restored from cold storage

*lDateFmt*
:   SQL Server date format code (see Remarks in [IEdmVault11::CreateNewVault](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~CreateNewVault.html))

*lDisplayErrCode*
:   Not implemented

Populates the Restore coldstored file version dialog with data.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Init( _    ByVal poVault As IEdmVault5, _    ByVal lArcSrvID As System.Integer, _    ByVal eError As EdmGetOpError, _    ByVal bsFileName As System.String, _    ByVal lDocID As System.Integer, _    ByVal lVersionNo As System.Integer, _    ByVal lDateFmt As System.Integer, _    ByVal lDisplayErrCode As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Init(     IEdmVault5 poVault,    System.int lArcSrvID,    EdmGetOpError eError,    System.string bsFileName,    System.int lDocID,    System.int lVersionNo,    System.int lDateFmt,    System.int lDisplayErrCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Init(  &   IEdmVault5^ poVault, &   System.int lArcSrvID, &   EdmGetOpError eError, &   System.String^ bsFileName, &   System.int lDocID, &   System.int lVersionNo, &   System.int lDateFmt, &   System.int lDisplayErrCode ) ``` | |

#### Parameters

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); pointer to the vault

*lArcSrvID*
:   Archive server ID

*eError*
:   [EdmGetOpError](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetOpError.html); error code returned after getting coldstored version

*bsFileName*
:   Name of the file being restored from cold storage

*lDocID*
:   ID of the document being restored from cold storage

*lVersionNo*
:   Version number of the file being restored from cold storage

*lDateFmt*
:   SQL Server date format code (see Remarks in [IEdmVault11::CreateNewVault](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~CreateNewVault.html))

*lDisplayErrCode*
:   Not implemented

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmGetCSVersionDialog Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetCSVersionDialog.html)

[IEdmGetCSVersionDialog Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmGetCSVersionDialog_members.html)