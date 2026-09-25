<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5~GetVariable.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetVariable Method (IEdmVariableMgr5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVariableMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5.html) : GetVariable Method (IEdmVariableMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poIdOrName*
:   ID or name of variable to get

Gets a variable with the specified ID or name.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetVariable( _    ByRef poIdOrName As System.Object _ ) As IEdmVariable5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmVariable5 GetVariable(     ref System.object poIdOrName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmVariable5^ GetVariable(  &   System.Object^% poIdOrName ) ``` | |

#### Parameters

*poIdOrName*
:   ID or name of variable to get

#### Return Value

[IEdmVariable5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5.html); Null if poIdOrName is not valid

# ![](dotnetimages/collapse.gif)Example

[Batch Update Card Variables (VB.NET)](Batch_Update_Variables_Example_VBNET.htm)

[Batch Update Card Variables (C#)](Batch_Update_Variables_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

C++ users not using smart-pointer wrapper functions must release the returned pointer, IEdmVariable5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The variable name or ID is not recognized.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVariableMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5.html)

[IEdmVariableMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2