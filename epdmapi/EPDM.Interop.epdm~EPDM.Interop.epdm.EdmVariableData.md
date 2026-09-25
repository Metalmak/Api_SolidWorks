<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData.html -->

![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/collapse.gif)
![](dotnetimages/expand.gif)
![](dotnetimages/drpdown.gif)
![](dotnetimages/drpdown_orange.gif)
![](dotnetimages/copycode.gif)
![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |

| EdmVariableData Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmVariableData Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about a variable created with [IEdmVariableMgr6::AddVariables](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr6~AddVariables.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmVariableData     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmVariableData : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmVariableData : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmVariableData{
  string [mbsVariableName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData~mbsVariableName.html);
  EdmVariableType [meType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData~meType.html);
  integer [mlEdmVariableFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData~mlEdmVariableFlags.html);
  EdmAttributeData [mpoAttributes](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData~mpoAttributes.html);
  integer [mlVariableID](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData~mlVariableID.html);
};

# ![](dotnetimages/collapse.gif)Example

[Add Card Variables to Vault (VB.NET)](Add_Variables_to_Vault_Example_VBNET.htm)

[Add Card Variables to Vault (C#)](Add_Variables_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmVariableData Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007