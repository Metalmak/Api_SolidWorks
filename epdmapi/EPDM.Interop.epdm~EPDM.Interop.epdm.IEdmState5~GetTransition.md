<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~GetTransition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetTransition Method (IEdmState5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) : GetTransition Method (IEdmState5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsName*
:   Name of transition from this workflow state

Obsolete. Gets a transition from this workflow state by name.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetTransition( _    ByVal bsName As System.String _ ) As IEdmTransition5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmTransition5 GetTransition(     System.string bsName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmTransition5^ GetTransition(  &   System.String^ bsName ) ``` | |

#### Parameters

*bsName*
:   Name of transition from this workflow state

#### Return Value

[IEdmTransition5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTransition5.html); Null if no transition for bsName is found

# ![](dotnetimages/collapse.gif)Remarks

This method is not supported in SOLIDWORKS PDM Professional Version 6.0 and later, because workflows in SOLIDWORKS PDM Professional 6.0 may contain several transitions with the same name. In SOLIDWORKS PDM Professional Version 5.3, the user was forced to create transitions with unique names in the workflow editor. It is, therefore, no longer possible to uniquely identify transitions by name.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmTransition5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The transition is not found.* E\_NOTIMPL: This method is obsolete as of SOLIDWORKS PDM Professional Version 6.0.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html)

[IEdmState5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2