<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmBomType Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmBomType Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Types of BOM passed in [EdmBomInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomInfo.html) and [EdmBomLayout2](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBomLayout2.html) structures.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmBomType     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmBomType : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmBomType : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **Computed** | 0 = The BOM is computed (check in/out and workflow are not supported) |
| **ComputedActivated** | 1 = The BOM is computed, and the Activated checkbox is checked so the BOM appears in File Explorer |
| **ItemBOM** | 8 |
| **Saved** | 2 = The user has saved this BOM |
| **SWBOM** | 3 = SOLIDWORKS BOM |
| **SWBOMActivated** | 4 = SOLIDWORKS BOM, and the Activated checkbox is checked so the BOM appears in File Explorer |
| **SWBOMSaved** | 5 = The user has saved this SOLIDWORKS BOM |
| **UndefinedBOM** | 9 = BOM template |
| **WeldmentBOM** | 7 = Used as a weldment BOM in the preview |
| **WeldmentCutlist** | 6 = Used as a weldment cutlist in the preview |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)