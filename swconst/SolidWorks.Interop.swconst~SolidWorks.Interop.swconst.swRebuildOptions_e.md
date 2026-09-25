<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swRebuildOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swRebuildOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swRebuildOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Rebuild options. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swRebuildOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swRebuildOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swRebuildOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swRebuildOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCurrentSheetDisp** | 8 or 0x8; Drawing only; only rebuilds the display of the views on the current drawing sheet |
| **swForceRebuildAll** | 2 or 0x2; Assembly or drawing; Forces a rebuild of all geometry |
| **swRebuildAll** | 1 or 0x1; Assembly or drawing; rebuilds geometry that has not been regenerated |
| **swUpdateDirtyOnly** | 16 or 0x10; Drawing only; only rebuilds drawing views that are dirty when OR'd with swCurrentSheetDisp option |
| **swUpdateMates** | 4 or 0x4; Assembly only; only rebuilds mates, which is much faster than rebuilding the geometry. Especially useful for IComponent2::Transform2 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)