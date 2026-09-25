<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAttributeData.html -->

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

| EdmAttributeData Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAttributeData_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAttributeData Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Contains information about an attribute mapping in a variable ([EdmVariableData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableData.html)).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmAttributeData     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmAttributeData : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmAttributeData : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmAttributeData{
  string [mbsAttribName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAttributeData~mbsAttribName.html);
  string [mbsBlockName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAttributeData~mbsBlockName.html);
  string [mbsExtensions](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAttributeData~mbsExtensions.html);
};

# ![](dotnetimages/collapse.gif)Example

[Add Card Variables to Vault (VB.NET)](Add_Variables_to_Vault_Example_VBNET.htm)

[Add Card Variables to Vault (C#)](Add_Variables_to_Vault_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Used by [IEdmVariableMgr6::AddVariables](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr6~AddVariables.html) to create new variables.

# ![](dotnetimages/collapse.gif)See Also

####

[EdmAttributeData Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAttributeData_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007