<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6~GetDebugAddIns.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetDebugAddIns Method (IEdmAddInMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6.html) : GetDebugAddIns Method (IEdmAddInMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoAddIns*
:   Array of [EdmAddInInfo2 structures](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html); one structure for each debug add-in

Gets information about all of the add-ins that have been installed for debugging on this machine.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetDebugAddIns( _    ByRef ppoAddIns() As EdmAddInInfo2 _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetDebugAddIns(     out EdmAddInInfo2[] ppoAddIns ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetDebugAddIns(  &   [Out] array<EdmAddInInfo2>^ ppoAddIns ) ``` | |

#### Parameters

*ppoAddIns*
:   Array of [EdmAddInInfo2 structures](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInInfo2.html); one structure for each debug add-in

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddInMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

You can install add-ins for debugging either of two ways:

* Right-clicking the **Add-ins** node in the SOLIDWORKS PDM Professional Administration Tool and clicking **Debug Add-ins**.* Calling [IEdmAddInMgr6::InstallDebugAddIn](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6~InstallDebugAddIn.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6.html)

[IEdmAddInMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 6.4 of SOLIDWORKS PDM Professional