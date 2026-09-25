<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCreateSectionViewAtOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCreateSectionViewAtOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCreateSectionViewAtOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Options that affect the section view that is created. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCreateSectionViewAtOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCreateSectionViewAtOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCreateSectionViewAtOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCreateSectionViewAtOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCreateSectionView\_ChangeDirection** | 4 or 0x4; If set, then the direction of this section view is switched; if not set, then the direction of this section view is not switched |
| **swCreateSectionView\_CutSurfaceBodies** | 128 or 0x80: If set, then shows only the intersecting line of a surface in a section view |
| **swCreateSectionView\_DisplaySurfaceCut** | 32 or 0x20; If set, then only the surfaces cut by the section line apear in the section view; if not set, then all model surfaces appear in the section view |
| **swCreateSectionView\_ExcludeFasteners** | 64 or 0x40; If set, then fasteners are not included in the section view; if not set, then fasteners are included in the section view |
| **swCreateSectionView\_NotAligned** | 1 or 0x1; If set, then the section does not snap into alignment with the parent view; if not set, then the section snaps into alignment with the parent view |
| **swCreateSectionView\_OffsetSection** | 2 or 0x2; If set, then an aligned section view is created (two lines at an angle); if not set, a normal projection section view is created |
| **swCreateSectionView\_Partial** | 16 or 0x10; If set, then a partial section view is created; if not set, then a complete section view is created |
| **swCreateSectionView\_ScaleWithModel** | 8 or 0x8; If set, then the section view is scaled with the model; if not set, then the section view is not scaled with the model |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)