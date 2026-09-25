<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.swDimXpertMaterialConditionModifier_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| swDimXpertMaterialConditionModifier\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) : swDimXpertMaterialConditionModifier\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

DimXpert material condition modifiers.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swDimXpertMaterialConditionModifier_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swDimXpertMaterialConditionModifier_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swDimXpertMaterialConditionModifier_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swDimXpertMaterialConditionModifier_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swDimXpertMaterialConditionModifier\_unknown** | 0 |
| **swDimXpertMCM\_LMC** | 1 = Least material condition |
| **swDimXpertMCM\_MMC** | 2 = Maximum material condition |
| **swDimXpertMCM\_NoMCM** | 3 = No material condition modifier |
| **swDimXpertMCM\_RFS** | 4 = Regardless of feature size |

# ![](dotnetimages/collapse.gif)Remarks

The material condition modifiers of this enumeration can be applied to the tolerance or datums of a [geometric tolerance](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertTolerance.html) to set the least, maximum, and RFS material conditions for a feature. MMC, LMC, and RFS can be applied only to features of size, such as holes. Material condition modifiers of geometric tolerances are set by clicking the Geometric Tolerances icon on the DimXpert tool bar and selecting MCM symbols that map to the members of this enumeration as follows:

|  |  |
| --- | --- |
| **DimXpert MCM Symbol** | **Enumeration member** |
| L | swDimXpertMCM\_LMC |
| M | swDimXpertMCM\_MMC |
| (blank) | swDimXpertMCM\_NoMCM |
| S | swDimXpertMCM\_RFS |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html)