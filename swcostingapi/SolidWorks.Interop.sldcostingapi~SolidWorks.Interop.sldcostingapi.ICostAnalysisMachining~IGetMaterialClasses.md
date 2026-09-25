<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~IGetMaterialClasses.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| IGetMaterialClasses Method (ICostAnalysisMachining) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysisMachining Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining.html) : IGetMaterialClasses Method (ICostAnalysisMachining) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumClassNames*
:   Number of material classes

Gets the names of the material classes from the Costing template for this machining Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetMaterialClasses( _    ByVal NumClassNames As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysisMachining Dim NumClassNames As System.Integer Dim value As System.String   value = instance.IGetMaterialClasses(NumClassNames) ``` | |

| C# |  |
| --- | --- |
| ``` System.string IGetMaterialClasses(     System.int NumClassNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ IGetMaterialClasses(  &   System.int NumClassNames ) ``` | |

#### Parameters

*NumClassNames*
:   Number of material classes

#### Return Value

* in-process, unmanaged C++: Pointer to an array of strings of the names of the material classes

- VBA, VB.NET, C#, and C++/CLI: Not supported

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ICostAnalsyisMachining::GetMaterialClassesCount](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysisMachining~GetMaterialClassesCount.html) to get the NumClassNames value.

See [Getting Started](GettingStarted-swcostingapi.html) for details about Costing templates.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysisMachining Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining.html)

[ICostAnalysisMachining Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining_members.html)

[ICostAnalysisMachinging::GetMaterialClasses Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~GetMaterialClasses.html)

[ICostAnalysisMachinging::CurrentMaterialClass Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~CurrentMaterialClass.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2013 SP0