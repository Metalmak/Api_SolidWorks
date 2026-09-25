<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~GetToolbarItemIDs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetToolbarItemIDs Method (IEdmMenu5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html) : GetToolbarItemIDs Method (IEdmMenu5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetID*
:   Array of IDs (see **Remarks**)

Gets the toolbar buttons associated with the menu commands.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetToolbarItemIDs( _    ByRef ppoRetID() As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetToolbarItemIDs(     out System.int[] ppoRetID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetToolbarItemIDs(  &   [Out] System.array<int>^ ppoRetID ) ``` | |

#### Parameters

*ppoRetID*
:   Array of IDs (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

The toolbar buttons were added to SOLIDWORKS PDM Professional with the [EdmMenuFlags.EdmMenu\_HasToolbarButton](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html) flag specified in the call to [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html).

C++ programmers must remember to correctly create and destroy the returned SAFEARRAY of IDs to avoid errors.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html)

[IEdmMenu5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5_members.html)

[IEdmMenu6::GetItems Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu6~GetItems.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional