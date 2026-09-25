<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFileSaveWarning_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFileSaveWarning\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFileSaveWarning\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Values for File, Save warnings that can be returned from the IModelDoc2 Save methods. These warnings do not cause the File, Save operation to fail. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFileSaveWarning_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFileSaveWarning_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFileSaveWarning_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFileSaveWarning_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFileSaveWarning\_AnimatorCameraViews** | 128 or 0x80 |
| **swFileSaveWarning\_AnimatorFeatureEdits** | 16 or 0x10 |
| **swFileSaveWarning\_AnimatorLightEdits** | 64 or 0x40 |
| **swFileSaveWarning\_AnimatorNeedToSolve** | 8 or 0x8 |
| **swFileSaveWarning\_AnimatorSectionViews** | 256 or 0x100 |
| **swFileSaveWarning\_EdrwingsBadSelection** | 32 or 0x20 |
| **swFileSaveWarning\_MissingOLEObjects** | 512 or 0x200 |
| **swFileSaveWarning\_NeedsRebuild** | 2 or 0x2 |
| **swFileSaveWarning\_OpenedViewOnly** | 1024 or 0x400 |
| **swFileSaveWarning\_RebuildError** | 1 or 0x1 |
| **swFileSaveWarning\_ViewsNeedUpdate** | 4 or 0x4 |
| **swFileSaveWarning\_XmlInvalid** | 2048 or 0x800 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)