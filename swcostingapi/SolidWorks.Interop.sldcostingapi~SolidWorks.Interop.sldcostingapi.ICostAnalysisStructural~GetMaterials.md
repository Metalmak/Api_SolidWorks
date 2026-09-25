<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~GetMaterials.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| GetMaterials Method (ICostAnalysisStructural) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysisStructural Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html) : GetMaterials Method (ICostAnalysisStructural) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ClassName*
:   Name of the material class

Gets the names of the materials in the specified class from the Costing template for this structural Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMaterials( _    ByVal ClassName As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysisStructural Dim ClassName As System.String Dim value As System.Object   value = instance.GetMaterials(ClassName) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMaterials(     System.string ClassName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMaterials(  &   System.String^ ClassName ) ``` | |

#### Parameters

*ClassName*
:   Name of the material class

#### Return Value

Array of strings of the names of the materials in ClassName

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostAnalysisStructural::GetMaterials.

# ![](dotnetimages/collapse.gif)Example

See the [ICostAnalysisStructural](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysisStructural Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html)

[ICostAnalysisStructural Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural_members.html)

[ICostAnalysisStructural::GetMaterialClasses Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~GetMaterialClasses.html)

[ICostAnalysisStructural::GetMaterialClassesCount Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~GetMaterialClassesCount.html)

[ICostAnalysisStructural::GetMaterialCount Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~GetMaterialCount.html)

[ICostAnalysisStructural::CurrentMaterial Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentMaterial.html)

[ICostAnalysisStructural::CurrentMaterialClass Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentMaterialClass.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2015 SP0