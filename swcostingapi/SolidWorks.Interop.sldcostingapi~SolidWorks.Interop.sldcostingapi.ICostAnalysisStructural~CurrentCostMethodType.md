<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentCostMethodType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| CurrentCostMethodType Property (ICostAnalysisStructural) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysisStructural Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html) : CurrentCostMethodType Property (ICostAnalysisStructural) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the structural stock cost method in the Costing analysis for this structural Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CurrentCostMethodType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysisStructural Dim value As System.Integer   instance.CurrentCostMethodType = value   value = instance.CurrentCostMethodType ``` | |

| C# |  |
| --- | --- |
| ``` System.int CurrentCostMethodType {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int CurrentCostMethodType {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Type of structural stock cost method as defined by [swcStructuralStockCostType\_e](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.swcStructuralStockCostType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostAnalysisStructural::CurrentCostMethodType.

# ![](dotnetimages/collapse.gif)Example

See the [ICostAnalysisStructural](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Setting of a structural stock cost method must match the data in the template. For example, if the **cost per unit length** option is not available in the template, then setting this method to swcStructuralStockCostType\_e.swcStructuralStockCost\_PerUnitLength fails.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysisStructural Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html)

[ICostAnalysisStructural Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural_members.html)

[ICostAnalysisStructural::CurrentStockUnitLength Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentStockUnitLength.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2015 SP0