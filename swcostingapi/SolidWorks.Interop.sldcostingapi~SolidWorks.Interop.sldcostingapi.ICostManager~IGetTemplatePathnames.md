<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostManager~IGetTemplatePathnames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| IGetTemplatePathnames Method (ICostManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostManager Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostManager.html) : IGetTemplatePathnames Method (ICostManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CostingType*
:   Type of Costing analysis as defined in [swcCostingType\_e](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.swcCostingType_e.html)

*NumTemplates*
:   Number of Costing templates available for CostingType

Gets the paths and filenames of the Costing templates available for the specified type of Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetTemplatePathnames( _    ByVal CostingType As System.Integer, _    ByVal NumTemplates As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostManager Dim CostingType As System.Integer Dim NumTemplates As System.Integer Dim value As System.String   value = instance.IGetTemplatePathnames(CostingType, NumTemplates) ``` | |

| C# |  |
| --- | --- |
| ``` System.string IGetTemplatePathnames(     System.int CostingType,    System.int NumTemplates ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ IGetTemplatePathnames(  &   System.int CostingType, &   System.int NumTemplates ) ``` | |

#### Parameters

*CostingType*
:   Type of Costing analysis as defined in [swcCostingType\_e](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.swcCostingType_e.html)

*NumTemplates*
:   Number of Costing templates available for CostingType

#### Return Value

* in-process, unmanaged C++: Pointer to an array of strings of the paths and filenames of the Costing templates available for CostingType* VBA, VB.NET, C#, and C++/CLI: Not supported

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ICostManager::GetTemplateCount](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostManager~GetTemplateCount.html) to get the NumTemplates value.

See [Getting Started](GettingStarted-swcostingapi.html) for details about Costing templates.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostManager Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostManager.html)

[ICostManager Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostManager_members.html)

[ICostManager::GetTemplatePathnames Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostManager~GetTemplatePathnames.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2013 SP0