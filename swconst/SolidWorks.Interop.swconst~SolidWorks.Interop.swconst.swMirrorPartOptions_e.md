<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swMirrorPartOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swMirrorPartOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swMirrorPartOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Options for creating a mirror part. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swMirrorPartOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swMirrorPartOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swMirrorPartOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swMirrorPartOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swMirrorPartOptions\_ImportAbsorbedSketchs** | 32 or 0x20 |
| **swMirrorPartOptions\_ImportAxes** | 4 or 0x4 |
| **swMirrorPartOptions\_ImportBodyMaterial** | 32768 or 0x8000 |
| **swMirrorPartOptions\_ImportCoordinateSystem** | 256 or 0x100 |
| **swMirrorPartOptions\_ImportCosmeticThreads** | 16 or 0x10 |
| **swMirrorPartOptions\_ImportCustomProperties** | 128 or 0x80 |
| **swMirrorPartOptions\_ImportCutListProperties** | 2048 or 0x800 |
| **swMirrorPartOptions\_ImportDimXpertAnnotations** | 16384 or 0x4000 |
| **swMirrorPartOptions\_ImportHoleWizardData** | 1024 or 0x400 |
| **swMirrorPartOptions\_ImportIndProps** | 8192 or 0x2000 = Lets you edit the sheet-metal definition in the mirrored part, which updates the cut-list properties |
| **swMirrorPartOptions\_ImportModelDimensions** | 512 or 0x200 |
| **swMirrorPartOptions\_ImportPartMaterial** | 65536 or 0x10000 |
| **swMirrorPartOptions\_ImportPlanes** | 8 or 0x8 |
| **swMirrorPartOptions\_ImportSMInfo** | 4096 or 0x1000 = Transfers the sheet-metal and flat-pattern information from the original part to the mirrored part; e.g., fixed face, grain direction, bendlines, and bounding box |
| **swMirrorPartOptions\_ImportSolids** | 1 or 0x1 |
| **swMirrorPartOptions\_ImportSurfaces** | 2 or 0x2 |
| **swMirrorPartOptions\_ImportUnabsorbedSketchs** | 64 or 0x40 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)