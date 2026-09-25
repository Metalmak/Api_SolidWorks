<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmResolveAction.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmResolveAction Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmResolveAction Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of flags that you return to SOLIDWORKS PDM Professional from [IEdmCallback6::Resolve](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6~Resolve.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmResolveAction     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmResolveAction : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmResolveAction : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmra\_ClearUnique** | 2 = Clear the duplicated unique-constrained values |
| **Edmra\_CopySerial** | 4 = Copy existing serial number values from the source file |
| **Edmra\_CreateSerial** | 8 = Create new serial number values |
| **Edmra\_ForceGenerateSerial** | 128 = Force regeneration of serial numbers when values already exist; without the flag, SOLIDWORKS PDM Professional only generates values that are missing in the file |
| **Edmra\_KeepExistingSerialNumbers** | 32 = Do not replace existing serial numbers with new ones; SOLIDWORKS PDM Professional still creates serial numbers for empty fields; if this flag is not specified, SOLIDWORKS PDM Professional overwrites existing serial numbers with new ones |
| **Edmra\_Replace** | 1 = Replace existing file with the new one |
| **Edmra\_Skip** | 16 = Do not process this file |
| **Edmra\_UniqueVarDelayCheck** | 64 = Delay the unique variable check to next check in |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)