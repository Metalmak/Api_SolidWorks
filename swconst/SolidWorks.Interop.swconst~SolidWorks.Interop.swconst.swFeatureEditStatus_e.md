<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFeatureEditStatus_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFeatureEditStatus\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFeatureEditStatus\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Editing status of feature. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFeatureEditStatus_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFeatureEditStatus_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFeatureEditStatus_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFeatureEditStatus_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFeature\_Editable** | 0 or 0x0; Feature can be edited |
| **swFeature\_NonEditable** | 1 or 0x1; Feature cannot be edited |
| **swFeature\_UnderEditing** | 2 or 0x2; If the feature is a sketch, then the sketch is already being edited |

# ![](dotnetimages/collapse.gif)Remarks

Although swFeatureEditStatus\_e is a bitmask, you currently cannot combine its mutually exclusive enumerators.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)