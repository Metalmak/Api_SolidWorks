<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddHook.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddHook Method (IEdmCmdMgr5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCmdMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5.html) : AddHook Method (IEdmCmdMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eCmdType*
:   Types of event that trigger IEdmAddIn5::OnCmd as defined in [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html)

*poReserved*
:   Null; reserved for future use

Adds a hook that makes SOLIDWORKS PDM Professional call this add-in's implementation of [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html) whenever the specified events occur.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddHook( _    ByVal eCmdType As EdmCmdType, _    Optional ByVal poReserved As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddHook(     EdmCmdType eCmdType,    System.object poReserved ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddHook(  &   EdmCmdType eCmdType, &   System.Object^ poReserved ) ``` | |

#### Parameters

*eCmdType*
:   Types of event that trigger IEdmAddIn5::OnCmd as defined in [EdmCmdType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdType.html)

*poReserved*
:   Null; reserved for future use

# ![](dotnetimages/collapse.gif)Example

See [IEdmCmdMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCmdMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5.html)

[IEdmCmdMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2