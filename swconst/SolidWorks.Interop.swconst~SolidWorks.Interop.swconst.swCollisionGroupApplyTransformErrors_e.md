<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCollisionGroupApplyTransformErrors_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCollisionGroupApplyTransformErrors\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCollisionGroupApplyTransformErrors\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Errors when applying transforms to collision groups.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCollisionGroupApplyTransformErrors_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCollisionGroupApplyTransformErrors_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCollisionGroupApplyTransformErrors_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCollisionGroupApplyTransformErrors_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCollisionGroupApplyTransformErrors\_GroupRemoved** | 3 = The specified collision group is no longer available |
| **swCollisionGroupApplyTransformErrors\_InvalidTransforms** | 2 = Array of transforms contains a null pointer for one or more elements or a pointer to an object other than an IMathTransform |
| **swCollisionGroupApplyTransformErrors\_None** | 0 |
| **swCollisionGroupApplyTransformErrors\_SizeMismatch** | 1 = Array of transforms does not contain one IMathTransform for each component in the collision group |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)