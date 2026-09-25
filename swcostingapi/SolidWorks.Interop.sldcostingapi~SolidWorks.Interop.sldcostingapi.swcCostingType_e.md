<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.swcCostingType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| swcCostingType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) : swcCostingType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Costing types.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swcCostingType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swcCostingType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swcCostingType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swcCostingType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swcCostingType\_Common** | 0 = Common Costing analysis; i.e., costing common to all Costing analyses (see **Remarks**) |
| **swcCostingType\_Machining** | 2 = Machining Costing analysis; includes 3D printing, casting, machining, and plastic |
| **swcCostingType\_SheetMetal** | 1 = Sheet metal Costing analysis; includes machined plate and sheet metal |
| **swcCostingType\_Structural** | 3 = Structural Costing analysis; includes 3D printing, casting, machining, and plastic |

# ![](dotnetimages/collapse.gif)Remarks

A complete Costing analysis includes the common Costing analysis and a specific Costing analysis; i.e., machining, sheet metal, or structural.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html)