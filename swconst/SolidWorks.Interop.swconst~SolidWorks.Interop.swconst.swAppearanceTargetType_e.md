<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swAppearanceTargetType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swAppearanceTargetType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swAppearanceTargetType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Types of targets to which to apply a copied appearance.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swAppearanceTargetType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swAppearanceTargetType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swAppearanceTargetType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swAppearanceTargetType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAppearanceTargetAppearanceFilter** | 5 = All appearances in the model that match the appearance of the selected face are applied the copied appearance |
| **swAppearanceTargetBody** | 2 = The body of the selected face is applied the copied appearance |
| **swAppearanceTargetComponent** | 4 = The component of the selected face is applied the copied appearance |
| **swAppearanceTargetFace** | 0 = The selected face is applied the copied appearance |
| **swAppearanceTargetFeature** | 1 = The feature of the selected face is applied the copied appearance |
| **swAppearanceTargetPart** | 3 = The part of the selected face is applied the copied appearance |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)