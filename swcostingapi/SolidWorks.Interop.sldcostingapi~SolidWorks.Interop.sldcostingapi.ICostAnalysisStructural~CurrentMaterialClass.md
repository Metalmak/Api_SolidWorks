<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentMaterialClass.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| CurrentMaterialClass Property (ICostAnalysisStructural) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysisStructural Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html) : CurrentMaterialClass Property (ICostAnalysisStructural) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the name of the material class for this structural Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property CurrentMaterialClass As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysisStructural Dim value As System.String   instance.CurrentMaterialClass = value   value = instance.CurrentMaterialClass ``` | |

| C# |  |
| --- | --- |
| ``` System.string CurrentMaterialClass {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ CurrentMaterialClass {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

#### Property Value

Name of the material class

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostAnalysisStructural::CurrentMaterialClass.

# ![](dotnetimages/collapse.gif)Example

See the [ICostAnalysisStructural](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Setting this property could invalidate other settings, e.g., material and weldment stock profile.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysisStructural Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html)

[ICostAnalysisStructural Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural_members.html)

[ICostAnalysisStructural::GetMaterialClasses Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~GetMaterialClasses.html)

[ICostAnalysisStructural::GetMaterialClassesCount Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~GetMaterialClassesCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2015 SP0