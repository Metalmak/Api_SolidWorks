<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostingDefaults~SetMaterialName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| SetMaterialName Method (ICostingDefaults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostingDefaults Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostingDefaults.html) : SetMaterialName Method (ICostingDefaults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MethodType*
:   Manufacturing method as defined in [swcMethodType\_e](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.swcMethodType_e.html)

*MaterialName*
:   Name of default material for MethodType

Sets the name of the default material for the specified manufacturing method for this Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMaterialName( _    ByVal MethodType As System.Integer, _    ByVal MaterialName As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostingDefaults Dim MethodType As System.Integer Dim MaterialName As System.String   instance.SetMaterialName(MethodType, MaterialName) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMaterialName(     System.int MethodType,    System.string MaterialName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMaterialName(  &   System.int MethodType, &   System.String^ MaterialName ) ``` | |

#### Parameters

*MethodType*
:   Manufacturing method as defined in [swcMethodType\_e](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.swcMethodType_e.html)

*MaterialName*
:   Name of default material for MethodType

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostDefaults::SetMaterialName.

# ![](dotnetimages/collapse.gif)Example

See the [ICostingDefaults](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostingDefaults.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Changes made to default settings are saved to the registry and are applied in the next and subsequent Costing sessions.

# ![](dotnetimages/collapse.gif)See Also

####

[ICostingDefaults Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostingDefaults.html)

[ICostingDefaults Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostingDefaults_members.html)

[ICostingDefaults::GetMaterialName Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostingDefaults~GetMaterialName.html)

[ICostingDefaults::GetMaterialClass Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostingDefaults~GetMaterialClass.html)

[ICostingDefaults::SetMaterialClass Method ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostingDefaults~SetMaterialClass.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2015 SP0