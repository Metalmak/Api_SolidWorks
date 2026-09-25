<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFeatureFillSurfaceOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFeatureFillSurfaceOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFeatureFillSurfaceOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Feature fill surface options. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFeatureFillSurfaceOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFeatureFillSurfaceOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFeatureFillSurfaceOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFeatureFillSurfaceOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swMergeResult** | 4 or 0x4; Corresponds to IFillSurfaceFeatureData::Merge |
| **swOptimizeSurface** | 1 or 0x1; Optimize surface |
| **swReverseDirection** | 8 or 0x8; Corresponds to IFillSurfaceFeatureData::ReverseDirection |
| **swReverseSurface** | 16 or 0x10; Corresponds to IFillSurfaceFeatureData::ReverseSurface |
| **swTryToFormSolid** | 2 or 0x2; Corresponds to IFillSurfaceFeatureData::TryToFormSolid |

# ![](dotnetimages/collapse.gif)Remarks

Some options might not work because the topology of the surface fill to be created might not permit them. In these cases, the options are ignored.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)