<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~IGetStockTypes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| IGetStockTypes Method (ICostAnalysisMachining) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysisMachining Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining.html) : IGetStockTypes Method (ICostAnalysisMachining) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MaterialClass*
:   Name of the material class

*MaterialName*
:   Name of the material

*NumStockTypes*
:   Number of stock types defined for the specified material

Gets the stock types for the specified material from the Costing template for this machining Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetStockTypes( _    ByVal MaterialClass As System.String, _    ByVal MaterialName As System.String, _    ByVal NumStockTypes As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysisMachining Dim MaterialClass As System.String Dim MaterialName As System.String Dim NumStockTypes As System.Integer Dim value As System.Integer   value = instance.IGetStockTypes(MaterialClass, MaterialName, NumStockTypes) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetStockTypes(     System.string MaterialClass,    System.string MaterialName,    System.int NumStockTypes ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetStockTypes(  &   System.String^ MaterialClass, &   System.String^ MaterialName, &   System.int NumStockTypes ) ``` | |

#### Parameters

*MaterialClass*
:   Name of the material class

*MaterialName*
:   Name of the material

*NumStockTypes*
:   Number of stock types defined for the specified material

#### Return Value

* in-process, unmanaged C++: Pointer to an array of integers of the stock types of the specified material as defined in [swcStockType\_e](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.swcStockType_e.html)

* VBA, VB.NET, C#, and C++/CLI: Not supported

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ICostAnalysisMachining::GetStockTypeCount](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysisMachining~GetStockTypeCount.html) to get the NumStockTypes value.

See [Getting Started](GettingStarted-swcostingapi.html) for details about Costing templates.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysisMachining Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining.html)

[ICostAnalysisMachining Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining_members.html)

[ICostAnalysisMachining::GetStockTypes Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~GetStockTypes.html)

[ICostAnalysisMachining::CurrentStockType Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~CurrentStockType.html)

[ICostAnalysisMachining::IGetMaterialClasses Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~IGetMaterialClasses.html)

[ICostAnalysisMachining::IGetMaterials Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~IGetMaterials.html)

[ICostAnalysisMachining::GetMaterialClasses Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~GetMaterialClasses.html)

[ICostAnalysisMachining::GetMaterials Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~GetMaterials.html)

[ICostAnalysisMachining::CustomStockCostInfoType Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~CustomStockCostInfoType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2013 SP0