<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfoFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmAddInFileInfoFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAddInFileInfoFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of file in the add-in package used in [EdmAddInFileInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddInFileInfo.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmAddInFileInfoFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmAddInFileInfoFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmAddInFileInfoFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmAdfif\_AddInObject32** | 2 = File contains the 32-bit [IEdmAddIn5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) implementation; the code is used only in combination with EdmAdfif\_ComDLL32 |
| **EdmAdfif\_AddInObject64** | 8 = File contains the 64-bit [IEdmAddIn5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5.html) implementation; the code is used only in combination with EdmAdfif\_ComDLL64 |
| **EdmAdfif\_ComDll32** | 1 = File should be COM-registered in a 32-bit process |
| **EdmAdfif\_ComDll64** | 4 = File should be COM-registered in a 64-bit process |
| **EdmAdfif\_DataFile** | 0 = Data file that is copied and maintained but not otherwise used by SOLIDWORKS PDM Professional |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)