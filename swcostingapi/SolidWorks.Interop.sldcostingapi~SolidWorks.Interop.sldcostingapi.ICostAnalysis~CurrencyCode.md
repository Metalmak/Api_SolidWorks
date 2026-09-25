<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~CurrencyCode.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| CurrencyCode Property (ICostAnalysis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysis Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis.html) : CurrencyCode Property (ICostAnalysis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the 3-letter currency code from the Costing template for this Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property CurrencyCode As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysis Dim value As System.String   value = instance.CurrencyCode ``` | |

| C# |  |
| --- | --- |
| ``` System.string CurrencyCode {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ CurrencyCode {    System.String^ get(); } ``` | |

#### Property Value

3-letter currency code

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostAnalysis::CurrencyCode.

# ![](dotnetimages/collapse.gif)Example

[Create Sheet Metal Costing Analysis (C#)](Create_Sheet_Metal_Costing_Analyses_Example_CSharp.htm)

[Create Sheet Metal Costing Analysis (VB.NET)](Create_Sheet_Metal_Costing_Analyses_Example_VBNET.htm)

[Create Sheet Metal Costing Analysis (VBA)](Create_Sheet_Metal_Costing_Analyses_Example_VB.htm)

[Create Machining Costing Analysis (C#)](Create_Machining_Costing_Analyses_Example_CSharp.htm)

[Create Machining Costing Analysis (VB.NET)](Create_Machining_Costing_Analyses_Example_VBNET.htm)

[Create Machining Costing Analysis (VBA)](Create_Machining_Costing_Analyses_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Examples of 3-letter currency codes are:

* **USD** for United States Dollars* **EUR** for Euros* **GBP** for British Pounds* etc.

See [Getting Started](GettingStarted-swcostingapi.html) for details about Costing templates.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysis Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis.html)

[ICostAnalysis Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis_members.html)

[ICostAnalysis::CurrencyName Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~CurrencyName.html)

[ICostAnalysis::CurrencySeparator Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis~CurrencySeparator.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2013 SP0