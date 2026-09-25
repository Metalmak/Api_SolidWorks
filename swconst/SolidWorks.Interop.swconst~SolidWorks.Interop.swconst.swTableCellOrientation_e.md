<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swTableCellOrientation_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swTableCellOrientation\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swTableCellOrientation\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Orientations of text in table cells.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swTableCellOrientation_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swTableCellOrientation_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swTableCellOrientation_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swTableCellOrientation_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swTableCellOrientation\_Down** | 3 |
| **swTableCellOrientation\_Left** | 1 |
| **swTableCellOrientation\_Right** | 0 |
| **swTableCellOrientation\_Rotate90CCW** | 6 = Rotate text 90 degrees counter clockwise from the current orientation |
| **swTableCellOrientation\_Rotate90CW** | 5 = Rotate text 90 degrees clockwise from the current orientation |
| **swTableCellOrientation\_Up** | 2 |
| **swTableCellOrientation\_Varies** | 4 = Orientation varies in several table cells; not valid when calling ITableAnnotation::SetCellTextOrientation |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)