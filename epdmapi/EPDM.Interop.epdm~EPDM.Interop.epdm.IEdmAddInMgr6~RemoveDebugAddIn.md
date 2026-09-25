<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6~RemoveDebugAddIn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RemoveDebugAddIn Method (IEdmAddInMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr6.html) : RemoveDebugAddIn Method (IEdmAddInMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oAddIn*
:   Contains either the path to the DLL of the add-in to remove or the ID of the class that implements [IEdmAddIn5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html)

Removes an add-in that has been installed for debugging.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RemoveDebugAddIn( _    ByVal oAddIn As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RemoveDebugAddIn(     System.object oAddIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RemoveDebugAddIn(  &   System.Object^ oAddIn ) ``` | |

#### Parameters

*oAddIn*
:   Contains either the path to the DLL of the add-in to remove or the ID of the class that implements [IEdmAddIn5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html)

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

Version 6.4 of SOLIDWORKS PDM Professional or later