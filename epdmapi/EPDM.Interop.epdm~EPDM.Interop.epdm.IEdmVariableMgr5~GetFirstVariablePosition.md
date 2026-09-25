<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5~GetFirstVariablePosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstVariablePosition Method (IEdmVariableMgr5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVariableMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5.html) : GetFirstVariablePosition Method (IEdmVariableMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Starts an enumeration of the variables in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstVariablePosition() As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstVariablePosition() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstVariablePosition(); ``` | |

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first variable in the enumeration

# ![](dotnetimages/collapse.gif)Example

[Find Data Cards with Description Variable (C#)](Find_Data_Cards_with_Description_Variable_Example_CSharp.htm)

[Find Data Cards with Description Variable (VB.NET)](Find_Data_Cards_with_Description_Variable_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, pass the returned position of the first variable to [IEdmVariableMgr5::GetNextVariable](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5~GetNextVariable.html) to get the first variable in this list. Then call IEdmVariableMgr5::GetNextVariable repeatedly to get the rest of the variables.

C++ users not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVariableMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5.html)

[IEdmVariableMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2