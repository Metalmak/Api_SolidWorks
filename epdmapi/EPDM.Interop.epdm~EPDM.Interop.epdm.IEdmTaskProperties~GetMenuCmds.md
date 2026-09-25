<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~GetMenuCmds.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetMenuCmds Method (IEdmTaskProperties) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html) : GetMenuCmds Method (IEdmTaskProperties) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoCmds*
:   Array of [EdmTaskMenuCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd.html) structures; one structure for each menu command

Gets the menu commands set with [IEdmTaskProperties::SetMenuCmds](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties~SetMenuCmds.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetMenuCmds( _    ByRef ppoCmds() As EdmTaskMenuCmd _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetMenuCmds(     out EdmTaskMenuCmd[] ppoCmds ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetMenuCmds(  &   [Out] array<EdmTaskMenuCmd>^ ppoCmds ) ``` | |

#### Parameters

*ppoCmds*
:   Array of [EdmTaskMenuCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmTaskMenuCmd.html) structures; one structure for each menu command

# ![](dotnetimages/collapse.gif)Remarks

The menu commands display in a File Explorer context menu.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmTaskProperties Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties.html)

[IEdmTaskProperties Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmTaskProperties_members.html)

[Task Add-in Sample](TaskSample.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010