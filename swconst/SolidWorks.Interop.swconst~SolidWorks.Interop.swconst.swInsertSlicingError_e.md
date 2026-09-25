<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swInsertSlicingError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swInsertSlicingError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swInsertSlicingError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Error codes for slicing insertion. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swInsertSlicingError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swInsertSlicingError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swInsertSlicingError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swInsertSlicingError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swInsertSlicingError\_EntitiesCannotFormPlane** | 0x10 = Point and provided line overlap |
| **swInsertSlicingError\_GenericError** | 0x1 = Slicing inserted successfully |
| **swInsertSlicingError\_InvalidNumberOfPlanes** | 0x80 = Number of planes must be <= 100 |
| **swInsertSlicingError\_InvalidSlicesToGenerateOption** | 0x4 = Slicing method specified in ISlicingData::SlicesToGenerate is not valid |
| **swInsertSlicingError\_InvalidSlicingData** | 0x40 = Null or invalid slicing data |
| **swInsertSlicingError\_InvalidSlicingPlaneEntities** | 0x8 = None or invalid type of entities specified |
| **swInsertSlicingError\_InvalidTotalAngle** | 0x2 = (ISlicingData::NumberOfPlanes \* ISlicingData::Offset) is invalid |
| **swInsertSlicingError\_NoBodiesInsideBox** | 0x20 = No bodies are inside the bounding box |
| **swInsertSlicingError\_NoError** | 0x0 = Slicing inserted successfully |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)