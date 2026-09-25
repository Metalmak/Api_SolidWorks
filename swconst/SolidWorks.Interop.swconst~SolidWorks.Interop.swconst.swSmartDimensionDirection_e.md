<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSmartDimensionDirection_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSmartDimensionDirection\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSmartDimensionDirection\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Smart dimension extension line directions or rapid dimensioning selector quadrants.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSmartDimensionDirection_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSmartDimensionDirection_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSmartDimensionDirection_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSmartDimensionDirection_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSmartDimensionDirection\_Down** | 3 |
| **swSmartDimensionDirection\_Left** | 2 |
| **swSmartDimensionDirection\_Right** | 0 |
| **swSmartDimensionDirection\_Up** | 1 |

# ![](dotnetimages/collapse.gif)Remarks

In parts, this enumerator is used to specify the extension line that is needed to unambiguously define the angle to dimension. In the user interface, a direction manipulator appears during dimensioning if selected entities do not fully specify the angle to dimension. This enumerator specifies the directions of that manipulator.

In drawings that have **Rapid dimensioning** turned on, this enumerator may be used to specify the quadrant or side of the entities to which to add the display dimension.

See IModelDocExtension::AddDimension.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)