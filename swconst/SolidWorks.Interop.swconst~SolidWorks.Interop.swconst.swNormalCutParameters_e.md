<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swNormalCutParameters_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swNormalCutParameters\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swNormalCutParameters\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sheet metal normal cut parameters.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swNormalCutParameters_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swNormalCutParameters_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swNormalCutParameters_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swNormalCutParameters_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swNormalCutExtent** | 0 = Cuts the maximum amount from the intersection profiles on the top and bottom of the sheet metal body |
| **swNormalCutOffsetPlane** | 1 = Adjusts the layer where the intersection curve intersects the sheet metal body; Select a reference plane or top or bottom face to define the offset plane and then either set ISMNormalCutFeatureData2::LinkToKFactor to true or set ISMNormalCutFeatureData2::LayerAdjustmentValue to a value between 0 and 1 to adjust the layer |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)