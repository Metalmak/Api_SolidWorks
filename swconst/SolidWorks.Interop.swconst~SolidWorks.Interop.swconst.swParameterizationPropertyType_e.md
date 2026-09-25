<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swParameterizationPropertyType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swParameterizationPropertyType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swParameterizationPropertyType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Properties of U and V parameters.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swParameterizationPropertyType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swParameterizationPropertyType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swParameterizationPropertyType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swParameterizationPropertyType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swParameterizationPropertyType\_AllDerivativesContinuous** | 13737 |
| **swParameterizationPropertyType\_AllDerivativesNotContinuous** | 13738 |
| **swParameterizationPropertyType\_BoundsCoincident** | 13746 = Bounds at the ends of the parameter range are coincident |
| **swParameterizationPropertyType\_Circular** | 13740 = The parameter represents an angle around a circle; A circle indicates that the other parameter is a constant |
| **swParameterizationPropertyType\_Linear** | 13739 = The parameter is proportional to the distance along a straight line; A straight line indicates that the other parameter is a constant |
| **swParameterizationPropertyType\_Periodic** | 13701 = Periodic parameterization |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)