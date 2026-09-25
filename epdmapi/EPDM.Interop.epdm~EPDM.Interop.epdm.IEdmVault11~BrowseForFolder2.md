<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~BrowseForFolder2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| BrowseForFolder2 Method (IEdmVault11) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : BrowseForFolder2 Method (IEdmVault11) |

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

*poDefaultFolder*
:   [IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html); default folder to browse

*lFlags*
:   Combination of [EdmBrowseForFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrowseForFolderFlag.html) bits

Displays a Browse for Folder dialog box in which the user can click a file or item folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function BrowseForFolder2( _    ByVal hParentWnd As System.Integer, _    ByVal bsMessage As System.String, _    ByVal poDefaultFolder As IEdmFolder5, _    ByVal lFlags As System.Integer _ ) As IEdmFolder5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmFolder5 BrowseForFolder2(     System.int hParentWnd,    System.string bsMessage,    IEdmFolder5 poDefaultFolder,    System.int lFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmFolder5^ BrowseForFolder2(  &   System.int hParentWnd, &   System.String^ bsMessage, &   IEdmFolder5^ poDefaultFolder, &   System.int lFlags ) ``` | |

#### Parameters

*hParentWnd*
:   Parent window handle

*bsMessage*
:   Message to display in the dialog box

*poDefaultFolder*
:   [IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html); default folder to browse

*lFlags*
:   Combination of [EdmBrowseForFolderFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBrowseForFolderFlag.html) bits

#### Return Value

[IEdmFolder5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5.html); Null if the user clicks **Cancel** (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

[Get and Set Item References (VB.NET)](Get_and_Set_Item_References_Example_VBNET.htm)

[Get and Set Item References (C#)](Get_and_Set_Item_References_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method supersedes [IEdmVault5::BrowseForFolder](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~BrowseForFolder.html) by providing the ability to select items.

C++ users must release the returned interface, IEdmFolder5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The user pressed **Cancel**.* E\_EDM\_NOT\_LOGGED\_IN: You must call [IEdmVault5::Login](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~Login.html) or [IEdmVault5::LoginAuto](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~LoginAuto.html) before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010