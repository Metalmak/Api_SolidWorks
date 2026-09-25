<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetAddInInfo Method (IEdmAddIn5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddIn5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) : GetAddInInfo Method (IEdmAddIn5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poInfo*
:   [EdmAddInInfo structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo.html); before returning this structure, populate it with information about your add-in; used by the [Administration Add-ins dialog](AdminDlg.htm) during add-in registration

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); pointer to the active vault

*poCmdMgr*
:   [IEdmCmdMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5.html); pointer to the command manager that you use to add hooks, menu commands, and toolbar buttons

Called by SOLIDWORKS PDM Professional to obtain information about this add-in and the commands it supports.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetAddInInfo( _    ByRef poInfo As EdmAddInInfo, _    ByVal poVault As IEdmVault5, _    ByVal poCmdMgr As IEdmCmdMgr5 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetAddInInfo(     out EdmAddInInfo poInfo,    IEdmVault5 poVault,    IEdmCmdMgr5 poCmdMgr ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetAddInInfo(  &   [Out] EdmAddInInfo poInfo, &   IEdmVault5^ poVault, &   IEdmCmdMgr5^ poCmdMgr ) ``` | |

#### Parameters

*poInfo*
:   [EdmAddInInfo structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo.html); before returning this structure, populate it with information about your add-in; used by the [Administration Add-ins dialog](AdminDlg.htm) during add-in registration

*poVault*
:   [IEdmVault5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html); pointer to the active vault

*poCmdMgr*
:   [IEdmCmdMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5.html); pointer to the command manager that you use to add hooks, menu commands, and toolbar buttons

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddin5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

See [IEdmAddIn5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) for more information.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddIn5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html)

[IEdmAddIn5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional