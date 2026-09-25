<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAutodimMark_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAutodimMark\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAutodimMark\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Selection mark values. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAutodimMark_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAutodimMark_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAutodimMark_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAutodimMark_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAutodimMarkEntities** | 1 or 0x1; Sketch entities to autodimension when [swAutodimEntitiesSelected](SOLIDWORKS.Interop.swconst~SOLIDWORKS.Interop.swconst.swAutodimEntities_e.html) is passed as the entitiesToDimension argument to ISketch::AutoDimension2 |
| **swAutodimMarkHorizontalDatum** | 2 or 0x2; Sketch entities to autodimension when [swAutodimEntitiesSelected](SOLIDWORKS.Interop.swconst~SOLIDWORKS.Interop.swconst.swAutodimEntities_e.html) is passed as the entitiesToDimension argument to ISketch::AutoDimension2 |
| **swAutodimMarkOriginDatum** | 8 or 0x8; Unique datum for the origin dimension scheme. Datum must be either a sketch point or a vertical sketch line. |
| **swAutodimMarkVerticalDatum** | 4 or 0x4; Unique datum for the horizontal dimension scheme; datum must be either a sketch point or a vertical sketch line |

# ![](dotnetimages/collapse.gif)Remarks

These values are passed by IModelDocExtension::SelectByID2.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)