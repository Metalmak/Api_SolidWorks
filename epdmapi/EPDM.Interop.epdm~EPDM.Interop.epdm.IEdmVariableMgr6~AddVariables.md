<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr6~AddVariables.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddVariables Method (IEdmVariableMgr6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVariableMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr6.html) : AddVariables Method (IEdmVariableMgr6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoVariables*
:   Array of [EdmVariableData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData.html) structures; one structure for each variable (see **Remarks**)

Adds the specified variables to the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddVariables( _    ByRef ppoVariables() As EdmVariableData _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddVariables(     out EdmVariableData[] ppoVariables ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddVariables(  &   [Out] array<EdmVariableData>^ ppoVariables ) ``` | |

#### Parameters

*ppoVariables*
:   Array of [EdmVariableData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData.html) structures; one structure for each variable (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmVariableMgr6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

In the ppoVariables structure, set mlVariableID to 0 before calling this method. The ID of the new variable is returned in mlVariableID.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVariableMgr6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr6.html)

[IEdmVariableMgr6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007