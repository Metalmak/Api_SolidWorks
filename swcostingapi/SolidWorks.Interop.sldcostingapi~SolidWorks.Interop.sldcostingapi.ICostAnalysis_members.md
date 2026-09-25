<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| ICostAnalysis Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) : ICostAnalysis Interface |

The following tables list the members exposed by [ICostAnalysis](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CostingTemplateName](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~CostingTemplateName.html) | Gets the name of the Costing template for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [CostingType](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~CostingType.html) | Gets the Costing type from the Costing template for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [CurrencyCode](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~CurrencyCode.html) | Gets the 3-letter currency code from the Costing template for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [CurrencyName](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~CurrencyName.html) | Gets the name of the currency from the Costing template for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [CurrencySeparator](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~CurrencySeparator.html) | Gets the delimiter for the currency from the Costing template for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [LengthUnit](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~LengthUnit.html) | Gets the unit for the length from the Costing template for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [LotSize](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~LotSize.html) | Gets or sets the quantity of parts to produce per batch for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [MarkUpPercent](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~MarkUpPercent.html) | Gets or sets the markup percentage for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [MarkUpType](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~MarkUpType.html) | Gets or sets the method of markup for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [MassUnit](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~MassUnit.html) | Gets the unit of mass from the Costing template for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [TotalQuantity](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~TotalQuantity.html) | Gets or sets the total quantity of parts to produce for this Costing analysis. |
| ![ Property](dotnetimages/Property.gif) | [UnitSystem](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~UnitSystem.html) | Gets the unit system from the Costing template for this Costing analysis. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetFirstCostFeature](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~GetFirstCostFeature.html) | Gets the first Costing feature in the CostingManager in this Costing analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetManufacturingCost](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~GetManufacturingCost.html) | Gets the total manufacturing cost in this Costing analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetMaterialCost](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~GetMaterialCost.html) | Gets the costs of the materials in this Costing analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetSetupCost](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~GetSetupCost.html) | Gets the tool setup cost in this Costing analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetSpecificAnalysis](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~GetSpecificAnalysis.html) | Gets the specific Costing analysis in this Costing analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetTotalCostToCharge](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~GetTotalCostToCharge.html) | Gets the total cost to charge the customer, including:   * [materials](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis~GetMaterialCost.html),* [manufacturing](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis~GetManufacturingCost.html),* [setup](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis~GetSetupCost.html),* [markup](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis~MarkUpPercent.html), and* [shop-rate](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysisMachining~ShopRate.html) costs    in this Costing analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetTotalCostToManufacture](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~GetTotalCostToManufacture.html) | Gets the total cost to manufacture the part:   * including [material](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis~GetMaterialCost.html), [manufacturing](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis~GetManufacturingCost.html), and [setup](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis~GetSetupCost.html) costs* excluding [markup](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysis~MarkUpPercent.html) and [shop-rate](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysisMachining~ShopRate.html) costs   in this Costing analysis. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysis Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis.html)

[SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html)