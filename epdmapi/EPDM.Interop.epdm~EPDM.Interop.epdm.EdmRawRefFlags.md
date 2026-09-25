<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawRefFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmRawRefFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRawRefFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Flags used in [EdmRawReference](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRawReference.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmRawRefFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmRawRefFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmRawRefFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Edmrrf\_Ghost** | 1 = DWG files can store grandchildren as references; for example, in the file tree: A.dwg=>B.dwg=>C.dwg the file C.dwg can be stored as a ghost reference in A.dwg and as a normal reference in B.dwg; SOLIDWORKS PDM Professional does not show ghost references in check-in dialog boxes but does update them when files are moved |
| **Edmrrf\_InternalComponent** | 2 = Not used |
| **Edmrrf\_Nothing** | 0 = Normal file reference |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)