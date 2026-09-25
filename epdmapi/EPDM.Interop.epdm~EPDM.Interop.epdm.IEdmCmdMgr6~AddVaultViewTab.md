<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr6~AddVaultViewTab.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddVaultViewTab Method (IEdmCmdMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCmdMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr6.html) : AddVaultViewTab Method (IEdmCmdMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hWnd*
:   Handle of the .NET control to display in the tab

*bsName*
:   Name of the tab

*bsIconPath*
:   Full path and filename of the 16X16 PNG image to display next to bsName on the tab

*bsToolTip*
:   Tool tip for the tab

*bsUniqueID*
:   Unique ID for this control

Adds the specified tab to the right of the tabs in the bottom panel of a vault view before opening it in File Explorer.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddVaultViewTab( _    ByVal hWnd As System.Long, _    ByVal bsName As System.String, _    ByVal bsIconPath As System.String, _    ByVal bsToolTip As System.String, _    ByVal bsUniqueID As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddVaultViewTab(     System.long hWnd,    System.string bsName,    System.string bsIconPath,    System.string bsToolTip,    System.string bsUniqueID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddVaultViewTab(  &   System.int64 hWnd, &   System.String^ bsName, &   System.String^ bsIconPath, &   System.String^ bsToolTip, &   System.String^ bsUniqueID ) ``` | |

#### Parameters

*hWnd*
:   Handle of the .NET control to display in the tab

*bsName*
:   Name of the tab

*bsIconPath*
:   Full path and filename of the 16X16 PNG image to display next to bsName on the tab

*bsToolTip*
:   Tool tip for the tab

*bsUniqueID*
:   Unique ID for this control

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCmdMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call this method in your add-in's implementation of [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) where you handle the [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html).EdmCmd\_PreExploreInit notification.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCmdMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr6.html)

[IEdmCmdMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018