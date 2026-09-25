<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| OnCmd Method (IEdmAddIn5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddIn5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) : OnCmd Method (IEdmAddIn5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poCmd*
:   [EdmCmd structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html); command information common to all affected files and folders

*ppoData*
:   Array of [EdmCmdData structures](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html), one for each affected file or folder

Called by SOLIDWORKS PDM Professional whenever one of the menu commands or hooks registered in [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html) is executed.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub OnCmd( _    ByRef poCmd As EdmCmd, _    ByRef ppoData() As EdmCmdData _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void OnCmd(     out EdmCmd poCmd,    out EdmCmdData[] ppoData ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnCmd(  &   [Out] EdmCmd poCmd, &   [Out] array<EdmCmdData>^ ppoData ) ``` | |

#### Parameters

*poCmd*
:   [EdmCmd structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html); command information common to all affected files and folders

*ppoData*
:   Array of [EdmCmdData structures](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html), one for each affected file or folder

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddin5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

See the [IEdmAddIn5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) topic for more information.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddIn5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html)

[IEdmAddIn5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional