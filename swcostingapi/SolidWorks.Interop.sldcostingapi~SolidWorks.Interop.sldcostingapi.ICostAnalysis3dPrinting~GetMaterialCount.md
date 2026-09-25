<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting~GetMaterialCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| GetMaterialCount Method (ICostAnalysis3dPrinting) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysis3dPrinting Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting.html) : GetMaterialCount Method (ICostAnalysis3dPrinting) |

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

Gets the number of materials in the specified material class from the Costing template for this 3D printing Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMaterialCount( _    ByVal ClassName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysis3dPrinting Dim ClassName As System.String Dim value As System.Integer   value = instance.GetMaterialCount(ClassName) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetMaterialCount(     System.string ClassName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetMaterialCount(  &   System.String^ ClassName ) ``` | |

#### Parameters

*ClassName*
:   Name of the material class

#### Return Value

Number of materials in ClassName

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostAnalysis3dPrinting::GetMaterialCount.

# ![](dotnetimages/collapse.gif)Example

See the [ICostAnalysis3dPrinting](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

See [Getting Started](GettingStarted-swcostingapi.html) for details about Costing templates.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysis3dPrinting Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting.html)

[ICostAnalysis3dPrinting Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting_members.html)

[ICostAnalysis3dPrinting::GetMaterials Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting~GetMaterials.html)

[ICostAnalysis3dPrinting::CurrentMaterial Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting~CurrentMaterial.html)

[ICostAnalysis3dPrinting::GetMaterialClasses Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting~GetMaterialClasses.html)

[ICostAnalysis3dPrinting::CurrentMaterialClass Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting~CurrentMaterialClass.html)

[ICostAnalysis3dPrinting::GetMaterialClassesCount Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysis3dPrinting~GetMaterialClassesCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2015 SP0