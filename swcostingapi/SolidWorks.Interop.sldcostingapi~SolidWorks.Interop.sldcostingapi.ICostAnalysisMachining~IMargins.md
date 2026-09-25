<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~IMargins.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| IMargins Property (ICostAnalysisMachining) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysisMachining Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining.html) : IMargins Property (ICostAnalysisMachining) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumDimensions*
:   Number of dimensions for the stock type

Gets or sets the margins for the [stock type](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysisMachining~CurrentStockType.html) for this machining Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property IMargins( _    ByVal NumDimensions As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysisMachining Dim NumDimensions As System.Integer Dim value As System.Double   instance.IMargins(NumDimensions) = value   value = instance.IMargins(NumDimensions) ``` | |

| C# |  |
| --- | --- |
| ``` System.double IMargins(     System.int NumDimensions ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double IMargins {    System.double get(System.int NumDimensions);    void set (System.int NumDimensions, System.double value); } ``` | |

#### Parameters

*NumDimensions*
:   Number of dimensions for the stock type

#### Property Value

* in-process, unmanaged C++: Pointer to an array of doubles of the available margins (see **Remarks**)

- VBA, VB.NET, C#, and C++/CLI: Not supported

# ![](dotnetimages/collapse.gif)Remarks

Before calling this property, call [ICostAnalysisMachining::GetMarginDimensionCount](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysisMachining~GetMarginDimensionCount.html) to get the NumMargins value.

The material determines the size of the array:

|  |  |
| --- | --- |
| **Material** | **Array** |
| Block | 6 doubles for the -X, +X, -Y, +Y, -Z, and +Z  [ICostAnalysisMachining::SpecificSizeEnabled](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysisMachining~SpecificSizeEnabled.html) must bet set to true to specify block dimensions to add to the tightest fitting stock faces. |
| Cylinder | 3 doubles for the -D, -L, and +L |
| Plate | 4 doubles, all 0, for the -W, +W, -L, and +L |

This property does not support setting margins:

* for plate material
   - or -* when a [custom size](SOLIDWORKS.Interop.sldcostingapi~SOLIDWORKS.Interop.sldcostingapi.ICostAnalysisMachining~IBlankSize.html) is defined.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysisMachining Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining.html)

[ICostAnalysisMachining Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining_members.html)

[ICostAnalysisMachining::Margins Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisMachining~Margins.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2013 SP0