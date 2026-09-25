<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetMenuCmds.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetMenuCmds Method (IEdmTaskProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html) : SetMenuCmds Method (IEdmTaskProperties) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poCmds*
:   Array of [EdmTaskMenuCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd.html) structures; one structure for each menu command to add to the context menus

Adds the specified menu commands to File Explorer context menus.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetMenuCmds( _    ByVal poCmds() As EdmTaskMenuCmd _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMenuCmds(     EdmTaskMenuCmd[] poCmds ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMenuCmds(  &   array<EdmTaskMenuCmd>^ poCmds ) ``` | |

#### Parameters

*poCmds*
:   Array of [EdmTaskMenuCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd.html) structures; one structure for each menu command to add to the context menus

# ![](dotnetimages/collapse.gif)Example

See the examples in [IEdmTaskProperties](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html).

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html)

[IEdmTaskProperties Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties_members.html)

[IEdmTaskProperties::GetMenuCmds Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetMenuCmds.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010