<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarVal.html -->

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

| EdmVarVal Structure | |
| [See Also](#seealsobookmark)  [Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarVal_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All Expand All  ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmVarVal Structure |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Passed to [IEdmBatchItemGeneration2::AddSelection2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration2~AddSelection2.html) to update a variable value.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Structure EdmVarVal     Inherits System.ValueType ``` | |

| C# |  |
| --- | --- |
| ``` public struct EdmVarVal : System.ValueType ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public value class EdmVarVal : public System.ValueType ``` | |

# ![](dotnetimages/collapse.gif)Example

struct EdmVarVal{
  integer [mlEdmVarValFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarVal~mlEdmVarValFlags.html);
  object [moVarIDorName](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarVal~moVarIDorName.html);
  object [moValue](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarVal~moValue.html);
};

# ![](dotnetimages/collapse.gif)Example

[Add Items (C#)](Add_Items_Example_CSharp.htm)

[Add Items (VB.NET)](Add_Items_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[EdmVarVal Members](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVarVal_members.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[Porgramming Items](Items.htm)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010