<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefFlags.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmRefFlags Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmRefFlags Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of item reference. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmRefFlags     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmRefFlags : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmRefFlags : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmRef\_Dynamic** | 4 = Auto-update item to file reference |
| **EdmRef\_File** | 1 = Item to file reference |
| **EdmRef\_Item** | 2 = Item to item reference |
| **EdmRef\_Static** | 8 = Attachment-type item to file reference |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)

[EdmItemRef Structure](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmItemRef.html)

[IEdmReference7::EdmRefFlags Property ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~EdmRefFlags.html)

[IEdmReference7::GetFirstChildPosition2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~GetFirstChildPosition2.html)

[IEdmReference7::GetFirstParentPosition2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmReference7~GetFirstParentPosition2.html)

[IEdmBatchItemGeneration2::AddSelection2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchItemGeneration2~AddSelection2.html)