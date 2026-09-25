<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAutodimEntities_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAutodimEntities\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAutodimEntities\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Entities to dimension ISketch::AutoDimension2 and IDrawingDoc::AutoDimension.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAutodimEntities_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAutodimEntities_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAutodimEntities_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAutodimEntities_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAutodimEntitiesAll** | 1 = Autodimensions all of the supported entities in the sketch |
| **swAutodimEntitiesBasedOnPreselect** | 0 = SOLIDWORKS to figure out what to do based on the selected supported entities marked with [swAutodimMarkEntities](SOLIDWORKS.Interop.swconst~SOLIDWORKS.Interop.swconst.swAutodimMark_e.html). If any exist, then autodimension them, just like swAutodimEntitiesSelected. If none exist, then autodimension all supported entities, just like swAutodimEntitiesAll |
| **swAutodimEntitiesSelected** | 2 = Autodimensions selected supported entities marked with [swAutodimMarkEntities](SOLIDWORKS.Interop.swconst~SOLIDWORKS.Interop.swconst.swAutodimMark_e.html). If none exist, then autodimensions all supported entities, just like swAutodimEntitiesAll |

# ![](dotnetimages/collapse.gif)Remarks

Supported entities are lines, points, vertices, faces, sketch entities, center lines, and center marks.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)