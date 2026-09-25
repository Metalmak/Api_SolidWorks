<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmVariableType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmVariableType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Constants that identify the data type of a variable.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmVariableType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmVariableType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmVariableType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmVarType\_Bool** | 4 = Boolean data (i.e., yes or no values) |
| **EdmVarType\_Date** | 5 = Date and time data |
| **EdmVarType\_Float** | 3 = Floating-point data (64 bit) |
| **EdmVarType\_Int** | 2 = Integer data (32 bit) |
| **EdmVarType\_None** | 0 = Error code; used internally |
| **EdmVarType\_Text** | 1 = String data |

# ![](dotnetimages/collapse.gif)Remarks

Used in [IEdmVariable5::VariableType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5~VariableType.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)