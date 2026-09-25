<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmVariableFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmVariableFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmVariableFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags that set the style of variables used in file and folder data cards. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmVariableFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmVariableFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmVariableFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmVar\_Mandatory** | 2 = Missing values are not permitted; only used for files, ignored for folders |
| **EdmVar\_Unique** | 1 = Values of the variable must be unique; only used for files, ignored for folders |
| **EdmVar\_VerFreeUpdateAll** | 4 = Every version and every revision, regardless access, workflow states etc., are affected by the variable update |
| **EdmVar\_VerFreeUpdateLatest** | 8 = Only the latest version is affected by the variable update |

# ![](dotnetimages/collapse.gif)Remarks

Used in [IEdmVariable5::Flags](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariable5~Flags.html).

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)