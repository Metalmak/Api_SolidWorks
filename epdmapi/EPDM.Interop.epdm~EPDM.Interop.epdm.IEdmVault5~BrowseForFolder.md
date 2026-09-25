<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~BrowseForFolder.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| BrowseForFolder Method (IEdmVault5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : BrowseForFolder Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParentWnd*
:   Parent window handle

*bsMessage*
:   Message to display in the dialog box

Obsolete. Superseded by [IEdmVault11::BrowseForFolder2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~BrowseForFolder2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function BrowseForFolder( _    ByVal hParentWnd As System.Integer, _    ByVal bsMessage As System.String _ ) As IEdmFolder5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmFolder5 BrowseForFolder(     System.int hParentWnd,    System.string bsMessage ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmFolder5^ BrowseForFolder(  &   System.int hParentWnd, &   System.String^ bsMessage ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle

*bsMessage*
:   Message to display in the dialog box

#### Return Value

[IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html); Null if the user clicks **Cancel** (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

C++ users must release the returned interface, IEdmFolder5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The user clicked **Cancel**.* E\_EDM\_NOT\_LOGGED\_IN: You must call [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) or [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2